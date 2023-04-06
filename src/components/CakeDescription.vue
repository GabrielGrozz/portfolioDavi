<template>
  <div class="description d-flex align-ites-center">
    {{ desc }}
  </div>
</template>

<script>
export default {
  name: "CakeDescription",
  props: {
    desc: String,
  },
};
</script>

<style scoped>
.description {
  margin: 30px 60px 0px 60px;
  width: 350px;
  height: 550px;
  border-radius: 5px;
  padding: 70px 50px;

  background: rgb(175, 175, 175);

  color: rgb(49, 49, 49);
  font-size: 1.5em;
  text-shadow: rgb(196, 196, 196) 3px 2px 1px;
  font-weight: bold;
}

@media screen and (max-width: 995px) {
  .description {
    height: 570px;
    margin: 25px 10px 0 45px;
    font-size: 1.2em;
  }
}

@media screen and (max-width: 895px) {
  .description {
    height: 570px;
    margin: 25px 30px 0 30px;
    font-size: 1.2em;
  }
}
@media screen and (max-width: 845px) {
  .description {
    height: 600px;
    margin: 25px 10px 0 45px;
    font-size: 1.2em;
  }
}

@media screen and (max-width: 730px) {
  .description {
    height: 500px;
    margin: 25px 0 0 0;
    border-radius: 0;
    font-size: 1.1em;
  }

  @media screen and (max-width: 655px) {
    .description {
      height: 580px;
      font-size: 1em;
    }
  }

  @media screen and (max-width: 615px) {
    .description {
      height: 45%;
      border-radius:  0;
      font-size: 1em;
    }
  }
}
</style>