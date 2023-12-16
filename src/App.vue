<script>
import NavbarMenu from "@/components/NavbarMenu/NavbarMenu.vue";
import BottomBarMenu from "@/components/BottomBarMenu/BottomBarMenu.vue";
export default {
  components: {
    NavbarMenu,
    BottomBarMenu,
  },
};
</script>

<template>
  <div class="container py-3">
    <nav class="media-desktop">
      <NavbarMenu />
    </nav>
  </div>
  <nav class="media-phone">
    <NavbarMenu />
  </nav>
  <div class="bottom--bar">
    <BottomBarMenu />
  </div>
</template>

<style scoped>
@media screen and (min-width: 768px) {
  .media-phone {
    display: none;
  }
}
@media screen and (max-width: 768px) {
  .container .media-desktop {
    display: none;
  }
}
@media screen and (min-width: 651epx) {
  .bottom--bar {
    display: none !important;
  }
}
.bottom--bar {
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 -3px 16px -13px black;
}
</style>
