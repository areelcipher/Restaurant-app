<template>
  <footer>
    <a href="mailto:fuudi@fuudi.com">fuudi@fuudi.com</a>
    <ul>
      <li>
        <a href="https://codepen.io" target="_blank">
          <i class="fab fa-codepen"></i>
        </a>
      </li>
      <li>
        <a href="http://dribbble.com" target="_blank">
          <i class="fab fa-dribbble"></i>
        </a>
      </li>
      <li>
        <a href="https://twitter.com" target="_blank">
          <i class="fab fa-twitter"></i>
        </a>
      </li>
      <li>
        <a href="https://github.com" target="_blank">
          <i class="fab fa-github"></i>
        </a>
      </li>
    </ul>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
footer {
  position: relative;
  top: 15vh;
  background: #111;
  color: #fff;
  text-align: center;
  padding: 2.5em 0;
  font-size: 16px;
}

footer a {
  color: inherit;
  text-decoration: none;
  font-weight: 800;
}

footer a:hover,
footer ul li a:hover {
  opacity: 0.7;
}

footer a:hover {
  text-decoration: underline;
}

footer ul {
  list-style: none;
  display: flex;
  justify-content: center;
  margin: 2em 0 0;
  padding: 0;
}

footer ul li{
  margin: 0 0.5em;
}

footer ul li a {
  padding: 0.5em;
}
</style>
