<template>
  <div class="home">
   <Banner />
  <section class="intro-section">
    <div class="intro-heading">
    <h4>We connect farmers directly with consumers</h4>
    <p>A lot of smallholder farmers are exploited by middlemen. We help link them directly to markets thus improving their margin!</p>
    </div>
    <div class="container">
        <div class="farmer__wrapper">
          <div class="farmer">
            <img src="../assets/farmer-icon.png" class="img-fluid intro-img" alt="">
            <h6>Connect with our farmers</h6>
            <p>A B2B market place for farmers to connect with buyers so middlemen can be eliminated and profits maximized for every harvest.</p>
          </div>
           <div class="farmer">
            <img src="../assets/money3.png" class="img-fluid intro-img" alt="">
            <h6>Grow your business</h6>
            <p>We provide the market for you so you can focus on doing what really matters, growing your business. Not only do we provide the market, we also provide technical and extension support.</p>
          </div>
           <div class="farmer">
            <img src="../assets/farmer-icon.png" class="img-fluid intro-img" alt="">
            <h6>Access to inputs and data</h6>
            <p>Our farmers also have access to improved farm inputs and data that is needed to improve productivity and enhance quality.</p>
          </div>
        </div>
    </div>
  </section>
  <!--End of Intro section
  ========================-->
  <!--Products section
  =========================-->
  <section class="products container-fluid">
    <div class="container">
      <div class="row">
        <div class="col-md-9">
          <h3>Do you plan to establish a modern farm?</h3>
          <p>With over 20 years of experience along the agricultural value chain, we are abe to ideate, plan and execute agro-allied projects of all sizes. It does not matter if it in tree/crops, animal husbandary, fisheries, agro-processing, our team of expert is able to execute beyound expectation. We follow best pratices in all our project execution and we give attention to details. We consider everything from seed quality to spacing to make sure we satisfy all your need.</p>
          <a href="tel:08103515205" class="product-btn">Contact Us</a>
        </div>
        <div class="col-md-3">
        </div>
      </div>
    </div>
  </section>
  <!--End of product section
  ==========================-->
  <!--Order section
  =========================-->
  <section class="order container-fluid">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <img src="../assets/palm.png" class="img-fluid order-img" alt="">
        </div>
         <div class="col-md-6 order-text">
          <h4>Order your palm products today!</h4>
          <p>Our primary products invloves all the products from the palm. From Crude Palm Oil to Palm Karnel, we can deliver to you in any part of Nigeria. We source the product from our partner farmers. Our quality is top notch and pricing is affordable.</p>
           <a href="tel:08103515205" class="order-btn">Order Now</a>
        </div>
      </div>
    </div>
  </section>
  <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from "@/components/Banner.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: 'home',
  components:{
    Banner,
    Footer
  }
}
</script>
