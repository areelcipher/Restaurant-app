<template>
  <div id="main-body">
    <Info id="info" />
    <Slider id="slider" />
    <Promo id="promo" />
    <Form />
  </div>
</template>

<script>
import Info from "./Info";
import Slider from "./Slider";
import Promo from "./Promo";
import Form from "./Form";
export default {
  components: {
    Info,
    Slider,
    Promo,
    Form
  }
};
</script>

<style scoped>
@media screen and (min-width: 700px) {
  #main-body {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  #promo {
    grid-area: 2/1/3/-1;
  }

  #info {
      position: relative;
      top: 35vh;
  }
}
</style>
