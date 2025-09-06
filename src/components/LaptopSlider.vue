<!-- <template>
    <div class="laptop-container">
      <div class="laptop">
        <div class="screen">
          <Swiper
            :modules="[Autoplay, Navigation, Pagination]"
            :slides-per-view="1"
            :loop="true"
            :autoplay="{ delay: 3000 }"
            :pagination="{ clickable: true }"
            class="swiper-container"
          >
            <SwiperSlide v-for="(image, index) in images" :key="index">
              <img :src="image" alt="Slide Image" />
            </SwiperSlide>
          </Swiper>
        </div>
        <div class="base"></div>
      </div>
    </div>
  </template>
  
  <script>
  import { Swiper, SwiperSlide } from "swiper/vue";
  import "swiper/css";
  import "swiper/css/navigation";
  import "swiper/css/pagination";
  import { Autoplay, Navigation, Pagination } from "swiper/modules";
  
  export default {
    components: { Swiper, SwiperSlide },
    setup() {
      const images = [
        "https://a.travel-assets.com/findyours-php/viewfinder/images/res40/481000/481689-Ocean-View-Norfolk.jpg",
        "https://static.vecteezy.com/system/resources/thumbnails/022/347/016/small_2x/aerial-view-beautiful-morning-view-from-indonesia-about-mountain-and-forest-photo.jpg",
        "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT4BFku8l4kCGi8ULk1c74vWrMu4g0i4wGpqA&s",
      ];
      return { images, Autoplay, Navigation, Pagination };
    },
  };
  </script>
  
  <style scoped>
  .laptop-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  .laptop {
    width: 400px;
    height: 280px;
    background: #222;
    border-radius: 10px;
    position: relative;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.5);
  }
  
  .screen {
    width: 90%;
    height: 70%;
    background: #000;
    border-radius: 5px;
    position: absolute;
    top: 10px;
    left: 5%;
    overflow: hidden;
  }
  
  .swiper-container img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  
  .base {
    width: 100%;
    height: 30px;
    background: #444;
    position: absolute;
    bottom: 0;
    border-radius: 0 0 10px 10px;
  }
  </style>
   -->

   <template>
    <div class="laptop-container">
      <div class="laptop">
        <img src="../assets/images/laptop_mockup.png" alt="Laptop Frame" class="laptop-frame" />
        <div class="screen">
          <Swiper
            :modules="[Autoplay, Navigation, Pagination]"
            :slides-per-view="1"
            :loop="true"
            :autoplay="{ delay: 3000 }"
            :pagination="{ clickable: true }"
            class="swiper-container"
          >
            <SwiperSlide v-for="(image, index) in images" :key="index">
              <img :src="image" alt="Slide Image" class="slide-image" />
            </SwiperSlide>
          </Swiper>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import { Swiper, SwiperSlide } from "swiper/vue";
  import "swiper/css";
  import "swiper/css/navigation";
  import "swiper/css/pagination";
  import { Autoplay, Navigation, Pagination } from "swiper/modules";
  
  export default {
    components: { Swiper, SwiperSlide },
    setup() {
        const images = [
        "https://a.travel-assets.com/findyours-php/viewfinder/images/res40/481000/481689-Ocean-View-Norfolk.jpg",
        "https://static.vecteezy.com/system/resources/thumbnails/022/347/016/small_2x/aerial-view-beautiful-morning-view-from-indonesia-about-mountain-and-forest-photo.jpg",
        "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT4BFku8l4kCGi8ULk1c74vWrMu4g0i4wGpqA&s",
      ];
      return { images, Autoplay, Navigation, Pagination };
    },
  };
  </script>
  
  <style scoped>
  .laptop-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  .laptop {
    position: relative;
    width: 500px;
    height: auto;
  }
  
  .laptop-frame {
    width: 100%;
    display: block;
  }
  
  .screen {
    position: absolute;
    top: 22%;
    right: 10%;
    /* left: 10%; */
    width: 80%;
    height: 50%;
    overflow: hidden;
  }
  
  .swiper-container {
    width: 90%;
    height: 88%;
  }
  
  .slide-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  </style>
  