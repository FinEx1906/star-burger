<script>
export default {
  data() {
    return {
      activeTab: "Asosiy",
    };
  },
  methods: {
    changeTab(tab) {
      this.activeTab = tab;
    },
  },
};
</script>

<template>
  <div class="navbar justify-content-between w-100">
    <button
      class="active"
      @click="changeTab('Asosiy')"
      :class="{ red: activeTab === 'Asosiy' }"
    >
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-home"></i>
        </section>
        <section>
          <span>Asosiy</span>
        </section>
      </div>
    </button>
    <button
      class="active"
      @click="changeTab('Sevimli')"
      :class="{ red: activeTab === 'Sevimli' }"
    >
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-heart"></i>
        </section>
        <section>
          <span>Sevimli</span>
        </section>
      </div>
    </button>
    <button
      class="active"
      @click="changeTab('Savat')"
      :class="{ red: activeTab === 'Savat' }"
    >
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-cart-shopping"></i>
        </section>
        <section>
          <span>Savat</span>
        </section>
      </div>
    </button>
    <button
      class="active"
      @click="changeTab('Kabinet')"
      :class="{ red: activeTab === 'Kabinet' }"
    >
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-user"></i>
        </section>
        <section>
          <span>Kabinet</span>
        </section>
      </div>
    </button>
  </div>
</template>

<style scoped>
.active {
  opacity: 0.6;
}
.active span {
  font-size: 17px;
}
.red {
  color: blue;
  transition: all 0.2s;
}
button {
  background: none;
  border: none;
  outline: none;
  cursor: pointer;
}
.navbar {
  padding: 20px;
  box-shadow: 0 -3px 16px -13px black;
  position: absolute;
  bottom: 0;
}
.navbar .link {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.navbar .active .link {
  font-size: 1rem !important;
}
</style>
