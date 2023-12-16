<script>
export default {};
</script>

<template>
  <div class="navbar justify-content-between w-100">
    <button class="active">
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-heart"></i>
        </section>
        <section>
          <span>Asosiy</span>
        </section>
      </div>
    </button>
    <button class="active">
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-home"></i>
        </section>
        <section>
          <span>Savat</span>
        </section>
      </div>
    </button>
    <button class="active">
      <div class="link fs-5">
        <section>
          <i class="fa text-center fs-4 fa-cart-shopping"></i>
        </section>
        <section>
          <span>Savat</span>
        </section>
      </div>
    </button>
    <button class="active">
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
  font-family: sans-serif;
  font-size: 17px;
}
button {
  background: none;
  border: none;
  outline: none;
  cursor: pointer;
}
.navbar {
  padding: 20px;
}
.navbar .link {
  display: flex;
  align-items: center;
  flex-direction: column;
}
</style>
