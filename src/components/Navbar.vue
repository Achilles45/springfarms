<template>
    <div class="navbar__wrapper container-fluid">
        <div class="container">
            <div class="navbar__contents d-flex justify-content-between">
                <div class="navbar__brand">
                     <router-link to="/" class="logo"><h4><i class="fas fa-unlock logo-icon"></i> Springfarms</h4></router-link>
                </div>
                 <div class="navbar__contents">
                     <ul class="navbar__items d-flex justify-content-between">
                         <li><router-link to="/about" class="nav-links">About</router-link></li>
      
                         <li><router-link to="/products" class="nav-links">Products</router-link></li>
                         <li><router-link to="/contact" class="nav-links contact-link">Contact</router-link></li>
                     </ul>
                 </div>
                 <div @click="openNav()" class="navbar-toggler">
                     <i class="fa fa-bars"></i>
                 </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Navbar',
    data(){
        return{

        }
    },
    methods: {
        openNav: function(){
            const nav = document.querySelector('.navbar__items');
            nav.classList.toggle('show-nav');
        }
    }
}
</script>
<style>

</style>
