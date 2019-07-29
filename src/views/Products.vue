<template>
    <div class="products__wrapper">
        <Navbar />
        <div class="products-heading">
            <div class="container">
                <h3 class="text-right">Products</h3>
            </div>
        </div>
        <div class="container-fluid mb-5">
            <div class="container">
                <div class="row mt-5">
                    <div class="col-12">
                        <h6>Our farmers glow and can provide you with anything ranging from palm products to poultry</h6>
                    </div>
                </div>
                <div class="row mt-3">
                    <div class="col-md-6 pb-3">
                        <img src="../assets/seedlings.jpg" class="img-fluid" alt="">
                    </div>
                     <div class="col-md-6">
                        <h4>Palm Seedlings</h4>
                        <p>We are able through the help of our partners, supply you with improved palm seedling that meets industry standards. Our seedlings are organically grown and thus, they are very healty and being abe to survive in all most any kind of environment</p>
                    </div>
                </div>
                 <div class="row mt-5">
                    <div class="col-md-6 pb-3">
                       <h4>Palm Oil</h4>
                       <p>Our palm oil is of high quality. We educate our partner farmers on best practices when it comes to oil palm processing. We can place deliver your orders to any location in Nigeria.</p>
                    </div>
                     <div class="col-md-6">
                           <img src="../assets/palm.png" class="img-fluid" alt="">
                    </div>
                </div>
                 <div class="row mt-5">
                    <div class="col-md-6 pb-3">
                       <img src="../assets/birds.jpg" class="img-fluid" alt="">
                    </div>
                     <div class="col-md-6">
                          <h4>Poultry Products</h4>
                          <p>Our modern poultry farm is coming soon! Watch this space</p>
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
    name: 'products',
    components:{
        Navbar,
        Footer
    }
}
</script>
<style>

</style>
