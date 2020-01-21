<template>
  <header>
    <!-- Logo -->
    <div id="logo">
      <h3>FUUDI</h3>
    </div>
    <!-- Nav -->
    <div id="nav-bar">
      <!-- Nav bar one -->
      <ul class="nav-one" :class="{ navOneOpen: navOpen }">
        <li @click="go"><a href="#order-form">ORDER ONLINE</a></li>
        <li @click="go"><a href="#order-form">PROMOTION</a></li>
        <li @click="go"><a href="#order-form">DELIVERY</a></li>
      </ul>
      <!-- Nav bar two -->
      <ul class="nav-two" :class="{ navOneOpen: navOpen }">
        <li @click="go"><a href="#promo">DESERTS</a></li>
        <li @click="go"><a href="#promo">SALADS</a></li>
        <li @click="go"><a href="#promo">OTHERS</a></li>
      </ul>
    </div>

    <!-- Burger Icon -->
    <div id="burger" @click="burger">
      <div class="bar-one" :class="{ burgerAnimOne: burgerAnim }"></div>
      <div class="bar-two" :class="{ burgerAnimTwo: burgerAnim }"></div>
      <div class="bar-three" :class="{ burgerAnimThree: burgerAnim }"></div>
    </div>
  </header>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      navOpen: false,
      burgerAnim: false
    };
  },
  methods: {
    burger() {
      (this.navOpen = !this.navOpen), (this.burgerAnim = !this.burgerAnim);
    },
    go() {
      this.navOpen = !this.navOpen;
      this.burgerAnim = false;
    }
  }
};
</script>

<style scoped>
/* Start of Header styling */
  header {
    position: fixed;
    background-color: #111;
    color: #fff;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 10vh;
    width: 100%;
    box-shadow: 1px 1px 3px #000;
    z-index: 1000;
  }

  #logo {
    width: 20%;
    margin-left: 20px;
  }

  #nav-bar {
    display: flex;
    width: 80%;
  }

  .nav-one {
    display: flex;
    justify-content: space-around;
    margin: 0;
    width: 100%;
    white-space: nowrap;
  }

  .nav-two {
    display: flex;
    justify-content: space-around;
    margin: 0;
    width: 100%;
    background-color: #fff;
  }

  .nav-one li, .nav-two li {
    list-style: none;
  }

  .nav-one li a {
    color: #fff;
  }

  .nav-two li a {
    color: #111;
    font-size: 14px;
  }

  .nav-two {
    position: absolute;
    right: 0;
    top: 10vh;
  }
  /* End of Header styling */

/* Styling for different screen sizes */
@media screen and (max-width: 700px) {
  header {
    position: fixed;
    background-color: #111;
    color: #fff;
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 10vh;
    width: 100%;
    box-shadow: 1px 1px 3px #000;
    z-index: 1000;
  }

  h3 {
    margin: 0;
  }

  li {
    list-style: none;
    width: 100%;
    height: 100%;
    /* display: block; */
    display: flex;
    justify-content: center;
    align-items: center;
    box-sizing: border-box;
    color: #fff;
  }

  .nav-two li a {
    color: #fff;
    font-size: 14px;
  }

  li:hover,
  li:focus,
  li:active {
    background-color: #111;
  }

  #burger {
    display: block;
    padding: 4px;
    z-index: 1000;
    margin-right: 20px;
  }

  .bar-one,
  .bar-two,
  .bar-three {
    width: 25px;
    height: 2px;
    background-color: #fff;
    transition: all 0.3s ease;
  }

  .bar-two,
  .bar-three {
    margin-top: 3px;
  }

  .nav-one {
    position: absolute;
    left: 0;
    top: 10vh;
    width: 50%;
    height: 90vh;
    background-color: #272727;
    color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: flex-start;
    padding: 0;
    transform: translateX(-100%);
    transition: transform 0.3s ease-in;
    z-index: 500;
  }

  .nav-two {
    position: absolute;
    right: 0;
    top: 10vh;
    width: 50%;
    height: 90vh;
    background-color: #272727;
    color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: flex-end;
    padding: 0;
    transform: translateX(100%);
    transition: transform 0.3s ease-in;
    z-index: 500;
  }
  .navOneOpen {
    transform: translateX(0%);
  }

  .navTwoOpen {
    transform: translateX(0%);
  }

  .burgerAnimOne {
    transform: rotate(-45deg) translate(-3px, 6px);
  }

  .burgerAnimTwo {
    opacity: 0;
  }

  .burgerAnimThree {
    transform: rotate(45deg) translate(0px, -5px);
  }

  .nav-one a {
    color: #fff;
  }

  .nav-two a {
    color: #fff;
  }
}
</style>
