
<template>
  
    <section class="home">
      <div class="overlay"></div>
      <div class="slides-container container">
        <div class="slide active">
          <div class="slide-content" data-aos="fade-right" style="overflow-x: hidden">
            <span>fresh and organic</span>
            <h3>upTo 50% off</h3>
            <button>shop now</button>
          </div>
          <div v-for="img in [index]" :key="img" class="slide-image">
            <img  :src="currentImg" alt="slide image">
          </div>
        </div>
      </div>
      <div @click="prev()" id="prev"><fontAwesome icon="arrow-left" /></div>
      <div @click="next()" id="next"><fontAwesome icon="arrow-right" /></div>
    </section>
  
    <section class="sales">
      <div class="container">
        <div class="sales-item" data-aos="fade-right" style="overflow-x: hidden">
          <div class="sales-details">
            <span>limited sales</span>
            <h3>upto 50% off</h3>
            <button>shop now</button>
          </div>
          <div class="sales-image" >
            <img src="../images/fruits.png" alt="fruits">
          </div>
        </div>
        <div class="sales-item" data-aos="fade-up">
          <div class="sales-details">
            <span>limited sales</span>
            <h3>upto 50% off</h3>
            <button>shop now</button>
          </div>
          <div class="sales-image">
            <img src="../images/fru.png" alt="fruits">
          </div>
        </div>
        <div class="sales-item" data-aos="fade-left">
          <div class="sales-details">
            <span>limited sales</span>
            <h3>upto 50% off</h3>
            <button>shop now</button>
          </div>
          <div class="sales-image">
            <img src="../images/juice.png" alt="fruits">
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
  data() {
    return {
      imgs: [
        "/healthy/assets/blackberry.png",
        "/healthy/assets/orange.png",
        "/healthy/assets/mango.png"],
      index: 0,
      timer: null
    }
    
  },
  mounted: function() {
    this.startSlide();
  },
  methods: {
    startSlide: function() {
      this.timer = setInterval(this.next, 50000);
    },
    next: function() {
      this.index +=1
    },
    prev: function() {
      this.index -=1
    },
  },

  computed: {
    currentImg: function() {
      return this.imgs[Math.abs(this.index)% this.imgs.length]
    }
  }
}



</script>