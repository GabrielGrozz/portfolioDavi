<template>
  <div
    :class="['name d-flex align-items-center justify-content-center p-5 mb-2']"
  >
    <slot class="slot"></slot>
  </div>
</template>

<script>
export default {
  name: "Cakename",
};
</script>

<style scoped>
.name {
  height: 100px;
  width: 45%;
  border-radius: 0 0 15px 0;
  background: rgb(186, 186, 186);
  box-shadow: rgba(0, 0, 0, 0.15) 5px 5px 2.6px;
}

@media screen and (max-width: 1100px) {
  .name {
    width: 53%;
  }
}
@media screen and (max-width: 953px) {
  .name {
    width: 63%;
  }
}
@media screen and (max-width: 804px) {
  .name {
    width: 83%;
  }
}
@media screen and (max-width: 615px) {
  .name {
    width: 100%;
    border-radius: 0;
  }
}
.name{
  font-size: .8em;
  height: 50px;

}
</style>