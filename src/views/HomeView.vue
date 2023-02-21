<template>
  <Banner />
  <div class="main-container">
    <h1>monte o seu burger:</h1>
    <BurgueForm />
  </div>
</template>
<script>
import Banner from "../components/Banner.vue";
import BurgueForm from "../components/BurguerForm.vue";
export default {
  name: "Home",
  components: {
    Banner,
    BurgueForm
  },
};
</script>
