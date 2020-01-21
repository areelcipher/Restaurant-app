<template>
  <div id="order-form">
    <p>Kindly fill in your details to order</p>
    <form action="">
      <form action="">
        <label for="name">Name</label>
        <input type="text" placeholder="Name" />
        <label for="email">Email</label>
        <input type="email" placeholder="e.g: fuudi@fuudi.com" />
        <label for="telephone">Telephone</label>
        <input type="text" placeholder="e.g: 080-Fuudi" />
        <label for="order">Your Order</label>
        <select name="" id="">
          <option value="">Select your Order</option>
          <option value="">Fried Rice with Chicken</option>
          <option value="">Jollof Rice with Coke</option>
          <option value="">Pizza with Ice Cream</option>
        </select>
        <input type="button" value="Enter" />
      </form>
    </form>
  </div>
</template>

<script>
export default {
  components: {}
};
</script>

<style>
#order-form {
  position: relative;
  top: 10vh;
  width: 100%;
  margin: 0 auto;
  background-color: #111;
}

#order-form p {
  margin: 30px auto 0 auto;
  font-weight: 600;
  font-size: 18px;
  background-color: #111;
  color: #fff;
  padding: 3px 5px;
  display: block;
  width: 93%;
  text-align: center;
}

#order-form form {
  display: grid;
  width: 95%;
  margin: 0 auto;
}

#order-form label {
  margin: 10px 0;
  color: #fff;
  font-weight: 300;
}

#order-form input,
#order-form select {
  margin-bottom: 10px;
  padding: 10px;
  border: none;
  outline: none;
  background: #272727;
  color: #fff;
}

#order-form select {
  background-color: #272727;
}

#order-form input[type="button"] {
  margin-top: 10px;
  background-color: #272727;
  color: #fff;
}

@media screen and (min-width: 700px) {
  #order-form {
    display: none;
  }
}
</style>
