<script>
import { RouterLink, RouterView } from "vue-router";
export default { name: "Navbar" };
</script>
<template>
  <div id="nav">
    <nav>
      <RouterLink to="/">
        <img src="" alt="" id="logo" />
      </RouterLink>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </div>

  <RouterView />
</template>
<style scoped></style>
