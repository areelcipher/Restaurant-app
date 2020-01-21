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
  width: 95%;
  margin: 0 auto;
}

#order-form p {
  margin: 50px 0 20px 0;
  font-weight: 600;
  font-size: 16px;
  background-color: #111;
  color: #fff;
  padding: 3px 5px;
  text-align: center;
  display: block;
  width: 100%;
}

#order-form form {
  display: grid;
  width: 95%;
  margin: 0 auto;
}

#order-form label {
  margin-bottom: 5px;
  color: #ff0000;
  font-weight: 500;
}

#order-form input,
#order-form select {
  margin-bottom: 10px;
  padding: 5px;
  border: 1px solid #111;
  outline: none;
}

#order-form select {
  background-color: #fff;
}

#order-form input[type="button"] {
  margin-top: 10px;
  background-color: #111;
  color: #fff;
}

@media screen and (min-width: 700px) {
  #order-form {
    display: none;
  }
}
</style>
