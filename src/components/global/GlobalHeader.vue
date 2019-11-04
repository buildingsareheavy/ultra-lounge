<template>
  <nav class="nav">
    <g-link class="nav__link" to="/">Home</g-link>
    <g-link class="nav__link" to="/about/">About</g-link>
  </nav>
</template>

<script>
export default {
  name: "global-header"
};
</script>

<style lang="scss">
.nav {
  display: flex;
  justify-content: flex-end;
  a {
    padding: 1em;
    text-decoration: none;
    color: black;
    transition: opacity 300ms;
    &:hover,
    &:focus {
      opacity: 0.7;
    }
  }
}
</style>