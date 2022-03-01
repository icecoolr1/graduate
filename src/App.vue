<template>
  <topbar></topbar>
  <Header></Header>
  <Pictures></Pictures>
  <main_content></main_content>
  <Footer></Footer>

</template>


<script>
import "./assets/vendor/purecounter/purecounter.js"
import "./assets/vendor/bootstrap/js/bootstrap.bundle.min.js"
import "./assets/vendor/glightbox/js/glightbox.min.js"
import "./assets/vendor/swiper/swiper-bundle.min.js"
import "./assets/vendor/php-email-form/validate.js"
import "./assets/js/main"

import Topbar from "@/components/Topbar";
import Header from "@/components/Header";
import Pictures from "@/components/Pictures";
import main_content from "@/components/main_content";
import Footer from "@/components/Footer";
export default {
  name: 'App',
  components: {
    Topbar,
    Header,
    Pictures,
    main_content,
    Footer
  }
}
</script>




<style>
@import "/src/assets/vendor/animate.css/animate.min.css";
@import "/src/assets/vendor/bootstrap/css/bootstrap.min.css";
@import "/src/assets/vendor/bootstrap-icons/bootstrap-icons.css";
@import "/src/assets/vendor/boxicons/css/boxicons.min.css";
@import "/src/assets/vendor/glightbox/css/glightbox.min.css";
@import "/src/assets/vendor/remixicon/remixicon.css";
@import "/src/assets/vendor/swiper/swiper-bundle.min.css";
@import "/src/assets/css/style.css";


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
