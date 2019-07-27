<template>
  <div class="about">
    <Navbar />
    <div class="about__contents container-fluid">
      <div class="container">
        <div class="row mt-5">
          <div class="col-12">
            <h3 class="about-head">About Us</h3>
            <p>Springfarms is an agro investment and trading agency that helps to connect smallholder farmers to markets. Her primary product of trade is along the palm value chain, from Crude Palm Oil, Palm Karnel Oil, Palm Karnel and everything in-between.
            Every harvest season, farmers are exploited largely due to available market and lack of information. We thought it fair that the farmer that laboured should enjoy the fruits of hs or her labour. Springfarmssolves this problem in two ways. We directly buy palm products from our partner farmers at a fair and competitive price and also connect them to other end users or industries.</p>
          </div>
        </div>
        <!--Why us section
        =====================-->
        <div class="row why-us">
        <div class="col-12">
          <h4>Why us</h4>
          <div class="row">
            <div class="col-md-4">
              <i class="fa fa-comments why-icon"></i>
              <h6>24/7 Support</h6>
              <p>We dont't leave our partner farmers or clients alone. Our support team is ready to provide all round support to ensure all forms of transactions are successful.</p>
            </div>
            <div class="col-md-4">
              <i class="fa fa-cubes why-icon"></i>
              <h6>Quality</h6>
              <p>We try to make sure all our partner farmers grow quality and healthy food that is free of inorganic chemicals to ensure our consumers are safe.</p>
            </div>
            <div class="col-md-4">
              <i class="fa fa-truck why-icon"></i>
              <h6>Effective Logistics</h6>
              <p>Don't worry about logistics when you transact with us. We have arranged a cheap but efficient means to take your orders to your doorteeps in record time.</p>
            </div>
          </div>
        </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: 'about',
  components:{
    Navbar,
    Footer
  }
}
</script>
