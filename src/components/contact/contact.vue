<template>
  <div class="container text-left">
    <div class="row my-auto h-100">
      <div class="col-md-5 col-7">
        <img src="../../assets/contact/contact-image.jpg" class="w-100 h-100" alt="">
      </div>
      <div class="my-auto col-md-5 col-5 position-relative">
        <div class="negativeMargin  bg-transparent pl-md-n5 font-weight-bold position-relative row">
          <h2 class="header text-dark">hello</h2>
        </div>
        <div class="row pl-md-5">
            my name is &nbsp;
          <p class="font-weight-bold"> Sthembiso Mashiyane</p>
          and I am currently watching &nbsp;
          <p class="font-weight-bold"> Paradise PD</p>
          <p class="pt-3">
            you can reach me on <br>
            tel: <a href="tel:079 228 2461">079 228 2461</a><br>
            email: <a
              href="mailto:sthembisomashiyane@gmail.com">sthembisomashiyane@gmail.com</a>
          </p>
          <p>
            Share :
            <a class="m-1" target="_blank" href="https://www.facebook.com/sthembiso.mashiyane"><i class="bi bi-facebook"></i></a>
            <a class="m-1" target="_blank" href="https://www.instagram.com/sthem_mash/"><i class="bi bi-instagram"></i></a>
          </p>
        </div>
      </div>
    </div>

  </div>
</template>
<script>


export default {
  name: "contact"
}
</script>

<style scoped>

.negativeMargin {
  margin-left: -40%;
}

.header {
  font-size: 15vw;
  background-color: transparent;
}

p {
  font-size: 1.3vw;
  margin-bottom: 0;
}

img{
  object-fit: cover;
}
</style>
