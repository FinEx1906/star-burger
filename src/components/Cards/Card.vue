<script>
export default {};
</script>
<template>
  <div class="col-sm-4 my-2 wrapper">
    <div class="card p-1">
      <div class="card-img">
        <img class="img-fluid" src="/Food Image.png" alt="error" />
      </div>
      <div class="card-content">
        <p class="food-name">Burger</p>
        <p class="food-gramm">250 gramm</p>
        <section class="d-flex">
          <h5>12.000 so'm</h5>
          <button>+</button>
        </section>
      </div>
    </div>
  </div>
</template>
<style scoped>
.wrapper .card .card-content p {
  margin: 3px 0;
}
.wrapper .card .card-content .food-name {
  color: #323142;
  font-size: 15.11px;
  font-weight: 400;
}
.wrapper .card .card-content .food-gramm {
  color: #323142;
  font-size: 13.11px;
  font-weight: 300;
}
.wrapper .card .card-content section {
  width: 100%;
  justify-content: space-between;
  display: flex;
}
.wrapper .card .card-content section h5 {
  color: #121826;
  font-size: 14.998px;
  font-weight: 500;
}
.wrapper .card .card-content section button {
  width: 28.909px;
  height: 19.816px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #323142;
  color: #fff;
  border: none;
  outline: none;
  border-radius: 0.25rem;
}
.wrapper .card {
  border: 1.444px solid var(--Colors-Gray-Gray-2, #f4f4f6);
  background: #fff;
  box-shadow: 4.865px 16.379px 36.189px 0px rgba(229, 229, 229, 0.7);
}
@media (max-width: 576px) {
  .wrapper {
    max-width: 180px;
  }
  .wrapper .card .card-content section button {
    width: 38.909px;
    height: 25.816px;
  }
}
@media (max-width: 350px) {
  .wrapper {
    max-width: 160px;
  }
  .wrapper .card .card-content section button {
    width: 30.909px;
    height: 20.816px;
  }
}

@media screen and (min-width: 992px) {
  .wrapper {
    max-width: 228px;
  }
}
</style>
