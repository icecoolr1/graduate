<template>
  <section id="hero">
    <div class="hero-container">
      <div id="heroCarousel" data-bs-interval="5000" class="carousel slide carousel-fade" data-bs-ride="carousel">

        <ol class="carousel-indicators" id="hero-carousel-indicators"></ol>

        <div class="carousel-inner" role="listbox">

          <!-- Slide 1 -->
          <div id="Slide1" class="carousel-item active" :class="isactive===0?'active':''">
            <div class="carousel-container">
              <div class="carousel-content">
                <h2 class="animate__animated animate__fadeInDown">欢迎来到<span><a style="color: #cff4fc">Idea</a></span><span><a style="color: #0dcaf0">School</a></span></h2>
                <p class="animate__animated animate__fadeInUp">尽精微，致广大</p>
                <a href="#about" class="btn-get-started scrollto animate__animated animate__fadeInUp">Read More</a>
              </div>
            </div>
          </div>

          <!-- Slide 2 -->
          <div id="Slide2" class="carousel-item " :class="isactive===1?'active':''">
            <div class="carousel-container">
              <div class="carousel-content">
                <h2 class="animate__animated animate__fadeInDown">卷</h2>
                <p class="animate__animated animate__fadeInUp">是一种态度</p>
                <a href="#about" class="btn-get-started scrollto animate__animated animate__fadeInUp">Read More</a>
              </div>
            </div>
          </div>

          <!-- Slide 3 -->
          <div id="Slide3" class="carousel-item" :class="isactive===2?'active':''">
            <div class="carousel-container">
              <div class="carousel-content">
                <h2 class="animate__animated animate__fadeInDown">学</h2>
                <p class="animate__animated animate__adeInUp">是一种活法</p>
                <a href="#about" class="btn-get-started scrollto animate__animated animate__fadeInUp">Read More</a>
              </div>
            </div>
          </div>

        </div>

        <a class="carousel-control-prev" href="#heroCarousel" role="button" data-bs-slide="prev"  @click="changePictureLeft">
          <span class="carousel-control-prev-icon ri-arrow-left-line" aria-hidden="true"></span>
        </a>

        <a class="carousel-control-next" href="#heroCarousel" role="button" data-bs-slide="next" @click="changePictureRight()">
          <span class="carousel-control-next-icon ri-arrow-right-line" aria-hidden="true"></span>
        </a>

      </div>
    </div>
  </section><!-- End Hero -->
</template>

<script>

export default {
  data(){
    return {
      list: [0,1,2],
      index: 0,
      isactive: 0,

    }
  },
  name: "pic_main",

  methods:{
    changePictureRight(){
      let a = this.isactive
      if(a!==2){
        a ++
      }
      this.isactive = a
    },


    changePictureLeft(){
      let a = this.isactive
      if(a!==0){
        a --
      }
      this.isactive = a

    }

  }

}
</script>

<style scoped>
@import "/src/assets/css/lpic.css";

</style>