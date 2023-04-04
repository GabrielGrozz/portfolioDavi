<template>
  <div class="main d-flex">
    <img class="cake img-thumbnail m-3" :src="cake" :alt="alt" />
  </div>
</template>

<script>
export default {
  name: "CakeContent",
  props: {
    cake: String,
    alt: String,
  },
};
</script>

<style scoped>
.main {
  height: 500px;
  padding-right: 50px;
  justify-content: end;
}

.cake {
  box-shadow: rgba(0, 0, 0, 0.15) 10px 10px 2.6px;
}

@media screen and (max-width: 1120px) {
  .cake {
    max-width: 280px;
    max-height: 280px;
  }
}
@media screen and (max-width: 953px) {
  .cake {
    max-width: 250px;
    max-height: 250px;
  }
}
@media screen and (max-width: 804px) {
  .cake {
    max-width: 200px;
    max-height: 200px;
  }
  .main {
    padding-right: 25px;
  }
}
@media screen and (max-width: 615px) {
  .cake {
    max-width: 290px;
    max-height: 290px;
    border-radius: 0;
  }
  .main {
    padding-right: 0;
    justify-content: center;
  }
}
</style>
