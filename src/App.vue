<script>
import NavbarMenu from '@/components/NavbarMenu/NavbarMenu.vue'
import BottomBarMenu from '@/components/BottomBarMenu/BottomBarMenu.vue'
export default {
  components: {
    NavbarMenu,
    BottomBarMenu
  }
}
</script>

<template>
  <div class="container py-3">
    <nav>
      <NavbarMenu />
    </nav>
    <div class="bottom--bar">
      <hr>
      <BottomBarMenu />
    </div>
  </div>
</template>

<style scoped>
.container .bottom--bar {
  display: flex;
  justify-content: center;
  align-items: center;
  position: fixed;

}
</style>