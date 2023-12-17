<script>
import NavbarMenu from "@/components/NavbarMenu/NavbarMenu.vue";
import BottomBarMenu from "@/components/BottomBarMenu/BottomBarMenu.vue";
import AdsSlide from "@/components/AdsSlider/AdsSlider.vue";
import Card from "@/components/Cards/Card.vue";
export default {
  components: {
    NavbarMenu,
    BottomBarMenu,
    AdsSlide,
    Card,
  },
};
</script>

<template>
  <div>
    <div class="container py-3">
      <nav class="media-desktop">
        <NavbarMenu />
      </nav>
      <div class="search">
        <label for="search">
          <i class="fa fa-search"></i>
        </label>
        <input type="search" placeholder="Mahsulotlarni izlang..." />
      </div>
    </div>
    <nav class="media-phone">
      <NavbarMenu />
    </nav>
    <div class="container">
      <AdsSlide />
      <div class="my-3">
        <h1>Burger</h1>
        <div class="row">
          <Card />
          <Card />
          <Card />
          <Card />
          <Card />
          <Card />
          <Card />
        </div>
      </div>
    </div>
    <div class="bottom--bar">
      <BottomBarMenu />
    </div>
  </div>
</template>

<style scoped>
.container .search {
  display: none;
}
.container .search input {
  width: 100%;
  background-color: #e9ecef;
  border: 1px solid #ced4da;
  border-radius: 0.25rem;
  padding: 5px 40px;
  color: #00000061;
  outline: none;
}
.container .search input::placeholder {
  color: #00000061;
}
.container .search label {
  display: block;
  position: absolute;
  transform: translate(10px, 7px);
  color: #00000061;
}
.bottom--bar {
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 -3px 16px -13px black;
}
@media screen and (min-width: 768px) {
  .media-phone {
    display: none;
  }
}
@media screen and (max-width: 375px) {
  .media-phone {
    display: none;
  }
  .container .search {
    display: block;
  }
}
@media screen and (max-width: 768px) {
  .container .media-desktop {
    display: none;
  }
}
@media screen and (min-width: 651px) {
  .bottom--bar {
    display: none !important;
  }
}
</style>
