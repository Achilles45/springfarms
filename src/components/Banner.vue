<template>
    <div class="banner__wrapper">
       <div class="container-fluid">
           <div class="container">
             <div class="navbar__wrapper d-flex justify-content-between">
                 <div class="navbar__logo">
                     <router-link to="/" class="logo"><h4><i class="fas fa-unlock logo-icon"></i> Springfarms</h4></router-link>
                 </div>
                 <div class="navbar__contents">
                     <ul class="navbar__items d-flex justify-content-between">
                         <li><router-link to="/" class="nav-links">About</router-link></li>
                         <li><router-link to="/" class="nav-links">Farmers</router-link></li>
                         <li><router-link to="/" class="nav-links">Farmshop</router-link></li>
                         <li><router-link to="/" class="nav-links">Consultancy</router-link></li>
                         <li><router-link to="/" class="nav-links contact-link">Contact</router-link></li>
                     </ul>
                 </div>
                 <div @click="openNav()" class="navbar-toggler">
                     <i class="fa fa-bars"></i>
                 </div>
             </div>
             <!--End of Hero-section
             ==========================-->
             <!--Hero section begins here
             ==========================-->
             <section class="hero-section">
                <div class="row">
                    <div class="col-md-7">
                       <h2>Connecting farmers to markets</h2>
                       <p>A lot of farm produce go to waste due to a number of reasons including lack of a strucutred market. We partner with smallholder farmers to connect them to markets...</p>
                       <router-link to="/about" class="hero-btn">Read More</router-link>
                    </div>
                    <div class="col-md-5">

                    </div>
                </div>
             </section>
           </div>
       </div>
    </div>
</template>
<script>
export default {
    name: 'Banner',
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
<style lang="scss" scoped>
@import '../styles/_colors.scss';
.banner__wrapper{
    background: linear-gradient(rgba(0, 0, 0, .7) rgba(0, 0, 0, .7)), url('../assets/farmer2.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    width: 100%;
    color: #fff;
    position: relative;
    .navbar__wrapper{
        padding-top: 2.6rem;
        .logo{
            color: #FFF;
            text-decoration: none;
            font-weight: bold;
            .logo-icon{
                color: $lightgreen;
            }
        }
        .navbar__contents{
            .navbar__items{
                .nav-links{
                    color: #FFF;
                    margin-left: 1rem;
                    text-decoration: none;
                    font-size: .899rem;
                    font-weight: bold;
                }
            }
             .contact-link{
                    background: transparent;
                    border: 1px solid #FFF;
                    padding: .6rem 2rem;
                    border-radius: 2px;
                    &:hover{
                        background: $lightgreen;
                        color: #FFF;
                        border: 1px solid $lightgreen;
                        transition: all ease-in-out .5s;
                    }
                }
        }
        .navbar-toggler{
            display: none;
        }
    }
}

//Hero-section
.hero-section{
    padding: 8rem 0;
    h2{
        font-family: 'Montserrat' !important;
        padding-top: 2.5rem;
        font-weight: bolder;
        padding-bottom: .5rem;
    }
    p{
        opacity: .7;
        line-height: 1.2;
        margin-bottom: 2rem;
        font-family: 'Montserrat' !important;
        font-size: .899rem;
    }
    .hero-btn{
        background: $lightgreen;
        color: #fff;
        text-decoration: none;
        padding: .9rem 2.5rem;
        text-align: center;
        border-radius: 2px;
        font-size: .899rem;
    }
}

//Media Queries
@media only screen and (max-width: 768px){
    .navbar__items{
        background: $lightgreen;
        position: absolute;
        flex-direction: column;
        padding: 4rem 2rem;
        top: 20%;
        right: -100%;
        border-radius: 4px;
        transition: all ease-in-out .5s;
        z-index: 2;
         .nav-links{
             line-height: 2;
         }
         .contact-link{
             line-height: 4;
         }
    }
    .show-nav{
        right: 10%;
    }
    .navbar-toggler{
        display: block !important;
        cursor: pointer;
    }
}
</style>
