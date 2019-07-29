<template>
    <div class="contact__wrapper">
        <Navbar />
        <div class="contact__heading">
            <div class="container">
            <h3 class="text-right">Contact Us</h3>
            </div>
        </div>
        <div class="container-fluid contact-details">
            <div class="container">
                <div class="row">
                   <div class="col-md-12">
                       <div class="row">
                           <div class="col-md-6">
                               <h5>We'd love to hear from you!</h5>
                               Reach out to the springfarms team anytime. Our support team will respond to your message within 24 hours!
                               <h6>Springfarms Headquarters</h6>
                               <p>By MTN mast, Ejemeh, Aniocha South LGA, Delta State, Nigeria.</p>
                               <h6>Phone</h6>
                               <p>09060245065</p>
                           </div>
                             <div class="col-md-6">
                                 <div v-if="error" class="alert alert-danger">
                                     {{ error }}
                                 </div>
                                 <div v-if="success" class="alert alert-success">
                                     {{ success }}
                                 </div>
                               <form @submit.prevent="submitForm()">
                                   <div class="row">
                                       <div class="col-md-6">
                                           <div class="form-group">
                                               <label for="fname">First Name</label>
                                               <input type="text" class="form-control" autocomplete="off" v-model="fname">
                                           </div>
                                       </div>
                                       <div class="col-md-6">
                                           <div class="form-group">
                                               <label for="lnmae">Last Name *</label>
                                               <input type="text" class="form-control" autocomplete="off" v-model="lname">
                                           </div>
                                       </div>
                                   </div>
                                   <div class="form-group">
                                               <label for="email">Email Address *</label>
                                               <input type="email" class="form-control" autocomplete="off" v-model="email">
                                           </div>
                                         <div class="form-group">
                                             <textarea class="message form-control" placeholder="Message Here ..." v-model="message"></textarea>
                                         </div>
                                         <button type="submit" class="form-btn">Submit</button>
                               </form>
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
import { setTimeout } from 'timers';
export default {
    name: 'contact',
    components:{
        Navbar,
        Footer
    },
    data(){
        return{
            fname: null,
            lname: null,
            email: null,
            message: null,
            error: null,
            success: null
        }
    },
    methods:{
        //Function to clear the error message after 3 seconds
        clearMsg: function(){
             const errMsg  = document.querySelector('.alert');
             errMsg.remove();
        },
        //Function to clear all fields
        clearFields: function(){
            this.fname = '';
            this.lname = '';
            this.email = '';
            this.message = '';
        },
        submitForm: function(){
           if(!this.fname || !this.lname || !this.email || !this.message){
               this.error = "Pleaase fill in all fields"
               setTimeout(this.clearMsg, 3000);
           }else{
               this.success = "Thank you. We will reach you soon!"
                setTimeout(this.clearMsg, 3000);
                this.clearFields();
           }
        }
    }
}
</script>
<style>

</style>
