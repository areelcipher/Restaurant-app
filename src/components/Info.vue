<template>
  <div id="info">
    <h1>
      Hello <i>fellas</i> :)<br />
      we've got <strong>ONLINE ORDER</strong> for y'all
    </h1>
    <a href="#order-form">Click To Order</a>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#info {
  position: relative;
  top: 10vh;
  width: 100%;
  height: 260px;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  z-index: 500;
}

#info h1 {
  text-align: center;
  font-size: 30px;
  margin: 40px 0;
}

strong {
  color: #ff0000;
  font-size: 34px;
  display: block;
}

#info a {
  background-color: #111;
  color: #fff;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
}
</style>
