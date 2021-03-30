<template>
  <div class="container vh-100">
    <div class="slider h-100">
      <div class="slides my-auto pb-5">
        <div id="slide-1">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-2">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-3">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-4">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-5">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-6">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-7">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-8">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-9">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
        <div id="slide-10">
          <video type="video/mp4" class="w-100"
                 src="../assets/videos/Mercedes_Leon_stage.mp4" poster="../assets/posters/mercedez.jpg"></video>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoCarousel",
  data() {
    return {
      hover: false,
    };
  },
  mounted: function () {
    // eslint-disable-next-line no-undef
    $(document).ready(function () {
      // eslint-disable-next-line no-undef,no-unused-vars
      $("video").on("mouseover", function (event) {
        this.play();

        // eslint-disable-next-line no-unused-vars
      }).on('mouseout', function (event) {
        this.pause();
        this.currentTime = 0;
      });
    })
  },
  methods: {}
}
</script>

<style scoped lang="scss">
* {
  box-sizing: border-box;
}

.slider {
  width: 100%;
  text-align: center;
  overflow: hidden;

  > a {
    display: inline-flex;
    width: 1.5rem;
    height: 1.5rem;
    background: white;
    text-decoration: none;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    margin: 0 0 0.5rem 0;
    position: relative;

    &:active {
      top: 1px;
    }

    &:focus {
      background: #000;
    }
  }
}

.slides {
  display: flex;
  overflow-x: auto;
  scroll-snap-type: x mandatory;
  scroll-behavior: smooth;
  -webkit-overflow-scrolling: touch;

  &::-webkit-scrollbar {
    width: 10px;
    height: 10px;
  }

  &::-webkit-scrollbar-thumb {
    background: black;
  }

  &::-webkit-scrollbar-track {
    padding-right: 20%;
    padding-left: 20%;
    background: transparent;
  }

  > div {
    scroll-snap-align: start;
    flex-shrink: 0;
    width: 30%;
    height: 300px;
    margin-right: 5%;
    transform-origin: center center;
    transform: scale(1);
    transition: transform 0.5s;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 100px;
  }
}

.author-info {
  background: rgba(0, 0, 0, 0.75);
  color: white;
  padding: 0.75rem;
  text-align: center;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  margin: 0;

  a {
    color: white;
  }
}

img {
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

html {
  height: 100%;
  overflow: hidden;
}

body {
  height: 100%;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(to bottom, #74ABE2, #5563DE);
  font-family: 'Ropa Sans', sans-serif;
}

</style>

