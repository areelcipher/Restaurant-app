<template>
  <div id="promo">
    <h4>Delicious Delicacies</h4>
    <div id="promo-imgs">
      <img src="../assets/5.jpg" alt="" />
      <img src="../assets/6.jpg" alt="" />
      <img src="../assets/7.jpg" alt="" />
      <img src="../assets/8.jpg" alt="" />
      <img src="../assets/9.jpg" alt="" />
      <img src="../assets/10.jpg" alt="" />
      <img src="../assets/11.jpg" alt="" />
      <img src="../assets/12.jpg" alt="" />
      <img src="../assets/13.jpg" alt="" />
      <img src="../assets/14.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>

#promo {
  position: relative;
  top: 10vh;
  width: 95%;
  margin: 0 auto;
  z-index: 500;
}

#promo h4 {
    margin: 20px 0 10px 0;
    text-align: center;
    background-color: #111;
    color: #fff;
    padding: 5px 0;
    letter-spacing: 2px;
}

#promo-imgs {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 5px;
}

#promo img {
  width: 100%;
}
@media screen and (min-width: 700px) {
  #promo-imgs {
    grid-template-columns: 1fr 1fr 1fr;
  }
}
</style>
