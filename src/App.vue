<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    Navbar,
    Footer,
  },
  data() {
    return {
      // ANTES ESTAVA "./src/assets/logo.png"
      // SEGUNDO A DOCUMENTACAO DO VUE
      // DEVE COMECAR COM .
      // EXEMPLO ./img/logo.png => public/img/logo.png

      //@ É EQUIVALENTE A .src ENTAO SE QUISER IMPORTAR DA SRC
      // VOCE PODE USAR "@/assets/logo.png"
      //MAS TEM UMA DIFERENÇA ENTRE CARREGAR A IMAGEM NO SEU PROJETO
      // E DIZER AO COMPILADOR A ORIGEM DA IMAGEM ENTÃO TEM QUE LER A DOCUMENTACAO E PROCURAR AJUDA NO GOOGLE

      //https://cli.vuejs.org/guide/html-and-static-assets.html#static-assets-handling

      logo_src: "./img/logo.png",
      app_name: "Make Your Burger",
    };
  },
};
</script>
<style>
* {
  font-family: Helvetica, sans-serif;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.main-container {
  margin: 50px;
  min-height: 250px;
}
h1 {
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
