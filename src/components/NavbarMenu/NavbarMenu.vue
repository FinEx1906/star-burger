<script>
export default {};
</script>

<template>
  <div>
    <div class="navbar">
      <div class="logo" style="pointer-events: none">
        <img src="/Brand.svg" alt="Brand" />
      </div>
      <div
        class="location d-flex align-items-center"
        style="
          background-color: #dfdcf5;
          padding: 8px;
          gap: 8px;
          border-radius: 16px;
        "
      >
        <section class="icon">
          <img src="/icon/location.svg" alt="" />
        </section>
        <section class="text mx-1">
          <span
            style="color: #4e40a1; font-weight: 400; font-family: sans-serif"
            >Beruniy ko’chasi, 5</span
          >
        </section>
      </div>
      <div class="notification d-flex align-items-center">
        <section
          class="likes mx-2 d-flex align-items-center h6 justify-content-center"
          style="
            background-color: #dfdcf5;
            cursor: pointer;
            border-radius: 100%;
            width: 40px;
            height: 40px;
          "
        >
          <i class="fa fa-heart" style="color: #4e40a1"></i>
          <span
            class="badge position-absolute d-block d-flex justify-content-center align-items-center"
            style="
              transform: translate(15px, -25px);
              background-color: #4e40a1;
              border-radius: 100%;
              width: 30px;
              height: 30px;
            "
            >234</span
          >
        </section>
        <section
          class="shopping mx-2 d-flex align-items-center h6 justify-content-center"
          style="
            background-color: #dfdcf5;
            cursor: pointer;
            border-radius: 100%;
            width: 40px;
            height: 40px;
          "
        >
          <i class="fa-solid fa-cart-shopping" style="color: #4e40a1"></i>
          <span
            class="badge position-absolute d-block d-flex justify-content-center align-items-center"
            style="
              transform: translate(15px, -25px);
              background-color: #4e40a1;
              border-radius: 100%;
              width: 30px;
              height: 30px;
            "
            >234</span
          >
        </section>
        <section
          class="user-account mx-2 d-flex align-items-center h6 justify-content-center"
          style="
            background-color: #dfdcf5;
            cursor: pointer;
            border-radius: 100%;
            width: 40px;
            height: 40px;
          "
        >
          <i class="fa fa-user" style="color: #4e40a1"></i>
        </section>
      </div>
    </div>
    <hr />
  </div>
</template>

<style scoped>

@media (max-width: 768px) {
  .navbar {
    justify-content: space-between;
    padding: 10px;
  } 
  /* .navbar .notification{
    display: none !important;
  } */
}
@media (max-width: 650px) {
  .navbar .notification{
    display: none !important;
  }
}
</style>
