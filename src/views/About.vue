<template>
  <div class="about">
    <Navbar />
    <div class="about__contents">
      <div class="about__heading">
        <div class="container">
          <h3 class="text-right">About Us</h3>
        </div>
      </div>
      <div class="about__body container-fluid">
        <div class="container">
          <div class="row">
            <div class="col-12">
              <p>Springfarms is an agro-trading/investment agency. We help connect partner farmers directly to markets, and make some key investment in agricultural production ranging from oil palm production to poultry farming. Our team is made up of highly talented and experienced developers, agricultural researchers, investment advosors, agricultural extension expets.</p>
            </div>
          </div>
          <div class="row mt-4">
            <div class="col-12">
              <h4>What problem are we solving?</h4>
              <p>Every harvest season, smallholder farmers harves food that many times do not get to market, and even if it does, they are exploited by many middlemen so the farmers do not really have anything econoimic progress from farming activities.</p>
            </div>
          </div>
          <div class="row mt-4 mb-5">
            <div class="col-12">
              <h4>What we can do for farmers</h4>
              <div class="row mt-3 mb-3">
                <div class="col-md-4 farmers">
                  <i class="fa fa-users about-icons"></i>
                  <h6>Connection to markets</h6>
                  <p>Our B2B feature helps to link our partner farmers to markets that are competitive in pricing.</p>
                </div>
                <div class="col-md-4 farmers">
                  <i class="fa fa-eye about-icons"></i>
                  <h6>Extension services</h6>
                  <p>Our expert field agents are always available to provide our farmers with modern and effective extension services.</p>
                </div>
                <div class="col-md-4 farmers">
                  <i class="fa fa-cubes about-icons"></i>
                      <h6>Improved inputs</h6>
                      <p>Our partner farmers are able to access improved inputs ranging from seedlings to insecticides at a very subsidized rate.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    <Footer />
  </div>
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
