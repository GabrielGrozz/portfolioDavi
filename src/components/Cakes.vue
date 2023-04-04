<template>
  <div class="conatainer-fluid">
    <div :class="['container-fluid p-0', 'bg-color-' + color]">
      <CakeName
        ><h2 class="cake-name"><a :href=link >{{ name }}</a></h2></CakeName
      >
      <div class="cakes-container">
        <CakeDescription class="cake-desc" :desc="description" />
        <CakeContent
          :cake="cake"
          :alt="name"
          :class="['bg-color-' + color, 'cake-content']"
          id="cake-content"
        />
      </div>
    </div>
  </div>
</template>

<script>
import CakeName from "./CakeName.vue";
import CakeContent from "./CakeContent.vue";
import CakeDescription from "./CakeDescription.vue";

export default {
  name: "Cakes",
  data() {
    return {

    };
  },
  components: {
    CakeName,
    CakeContent,
    CakeDescription,
  },
  props: {
    cake: String,
    name: String,
    color: String,
    description: String,
    link: String
  },
};
</script>

<style scoped>
.container-fluid {
  border-top: rgb(186, 186, 186) 10px solid;
}

.cake-name {
  font-size: 2.5em;
  text-shadow: rgba(135, 135, 135, 0.4) 3px 2px 1px;
}

.cakes-container {
  display: flex;
  justify-content: space-between;
  height: 650px;
}

@media screen and (max-width: 615px) {
  .cakes-container {
    position: relative;
    display: flex;
    justify-content: center;
  }

  #cake-content {
    background-color: rgba(135, 135, 135, 0);
    position: absolute;
  }
  .cake-desc {
    margin-top: 300px;
  }
}
</style>