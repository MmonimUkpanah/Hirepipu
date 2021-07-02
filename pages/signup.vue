<template>
    <div class="login-1">
        
        
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-6 login-3">
                    
                </div>
                <div class="col-md-6">
                    <ValidationObserver v-slot="{ invalid }">
                        <form @submit.prevent="signUp">
                        
                        <div class="login-2">
                            <h2>Register For An Account!</h2>
                            <p>For the purpose of industry regulation, your details are required.</p>
                        <div class="grid">
                            <div class="form-group">
                            <label >Your full name*</label>
                            <ValidationProvider
                                v-slot="{ errors }"
                                name="name"
                                rules="required">
                            <input type="text" class="form-control" name="name" 
                            v-model="signup.username" required>
                            <span class="input-invalid-message">
                                {{ errors[0] }}
                            </span>
                            </ValidationProvider>
                        </div>
                        
                        
                        
                        
                        <div class="form-group">
                            <label>Email Address*</label>
                            <ValidationProvider
                                v-slot="{ errors }"
                                name="email"
                                rules="required|email">
                            <input type="email" class="form-control" @keydown.space.prevent 
                            v-model="signup.email" required>
                            <span class="input-invalid-message">
                                {{ errors[0] }}
                            </span>
                            </ValidationProvider>
                        </div>
                        
                        
                        
                        
                        <div class="form-group">
                            <label>Create password*</label>
                            <ValidationProvider rules="min:8|required" v-slot="{ errors }" vid="signup.password" name="password">
                            <input type="password" class="form-control" @keydown.space.prevent v-model="signup.password">
                            <span>{{ errors[0] }}</span>
                            </ValidationProvider>
                        </div>
                        <div class="form-group">
                            <label> Confirm password*</label>
                            <ValidationProvider rules="confirmed:signup.password|min:8|required" name="Confirm Password" v-slot="{ errors }">
                            <input type="password" class="form-control" @keydown.space.prevent v-model="signup.password2">
                            <span>{{ errors[0] }}</span>
                            </ValidationProvider>
                        </div>
                        </div>
                        
                       <!-- <div>
                           <p>By clicking Create Account, you agree to ForexHup's<a href="/terms"> Terms and Conditions</a></p>
                       </div> -->
                       
                        <button type="submit" :disabled="invalid" class="login">Register Account</button>
                
                        </div>
                        
                    </form>
                    </ValidationObserver>
                    
                    
                </div>
            </div>
        </div>
    </div>
</template>



<script>
import { ValidationObserver, ValidationProvider } from "vee-validate";
import ElementUI from 'element-ui';
import 'element-ui/lib/theme-chalk/index.css';
export default {
    auth: false,
    components: {
    ValidationObserver: ValidationObserver,
    ValidationProvider: ValidationProvider
  },
    data(){
        return{
            signup: {
                username:'',
                email: '',
                password: '',
                password2: ''
            }
            
        }
    },
    mounted(){
    
    },
    methods: {
    // async signUp() {
    //   try {
    //     let response = await this.$axios.post("https://deunionreserve.herokuapp.com/accounts/api/register/",this.signup);
    //     let user = response.data.user;
    //         this.$auth.$storage.setLocalStorage("user", user);
    //         let token = response.data.token;
    //         this.$auth.$storage.setLocalStorage("jwt", token);
        
    //     console.log(response)
    //     this.$message({
    //         message: "Account created successfully!",
    //         type: "success",
    //         });
    //         this.$router.push("/profile");
    //   } catch (err) {
    //     console.log(err)
    //     this.$message({
    //         message: "There was a problem creating your account. Please try again.",
    //         type: "warning",
    //         });
    //   }
    // }
     signUp()
        {
            
             this.$axios.post("https://deunionreserve.herokuapp.com/accounts/api/register/",this.signup)
            .then((res)=> {
             console.log(res)
              this.$message({
             message: "Account created successfully!",
            type: "success",
           });
           this.$auth.loginWith('local', { data: this.signup })
           
           this.$router.push("/profile");
          
            })
            .catch((error)=> {
            console.log(error)
            this.$message({
             message: "There was a problem creating your account. Please try again.",
            type: "warning",
            });
            
            
            })
            
         
        },
  }
    
}

</script>




<style scoped>
@font-face {
    font-family: DMSans;
    src: url("/font/DMSans-Regular.ttf");
    }
    *{
        font-family: 'DM Sans', sans-serif  !important;
        
    }
    .login-1{
        background: white;
        
    }
    form{
        background-color: #FFFFFF !important;
        border-radius: 24px;
        margin-top: 0rem;
    }
    .login-2{
        padding:2rem 4rem ;
        
    }
    
    form h2{
        color: #0272A2;
        font-size: 40px;
        font-weight: bold;
        margin-bottom: 1rem;
    }
    a{
        text-decoration: none;
        color: #0272A2;
    }
    .form-group input{
        background: #F9F9FA  !important;
        border-radius: 8px;
        padding: 8px 8px;
        margin-bottom: 1rem;
        width: 100%;
    }
    form label{
        color: #0272A2;
        font-weight: bold;
    }
    .login{
        width: 100%;
        padding: 8px 0;
        border: none;
        border-radius: 8px;
        color: white !important;
        background-color: #0272A2;
        margin-top: 1rem;
    }
    .login-3{
        background: url(/img/new/two.svg) center center/cover;
        height: 100vh;
        margin-top: -1px;
        
    }
    .login-3 h2{
        font-size: 45px;
        color: #01445F;

    }
    .nav-item{
        margin-left: 3rem;
    }
    .active{
        border-bottom: 1px solid #dee2e6  !important ;
    }
    a{
        color: black;
    }
    .small{
      display: none;
    }
    .nav1{
        margin-top: 1rem;
    
    }


    @media(max-width: 576px){
        form h2{
        color: white;
        font-size: 35px;
        font-weight: bold;
        margin-bottom: 2rem;
    }
        .login-1{
        padding-top: 10px;
        background: #F4FAFD;
        height: auto;
    }
    form{
        background-color: #FFFFFF !important;
        border-radius: 10px;
        margin-top: 2rem;
    }
    form label{
        color: white;
        font-weight: bold;
    }
    .login-2{
        padding:3rem 1rem ;
        background: url(/img/new/two.svg) center center/cover;
        height: auto;
    }
    .login{
        width: 100%;
        padding: 8px 0;
        border: none;
        border-radius: 8px;
        color: white !important;
        background-color:black;
        margin-top: 1rem;
    }
    .login-3{
        display: none;
        
    }
    .login-3 h2{
        font-size: 45px;
        color: white;

    }
    input{
        background: #F9F9FA;
        border-radius: 8px;
        padding: 8px 8px;
        margin-bottom: 1.5rem;
        width: 100%;
    }
    .grid{
        display: grid;
        grid-template-columns: 1fr;
    }
    .small{
      display:block
    }
    .big{
      display:none;
    }
    .active{
        border-bottom: none  !important ;
    }
    .nav-item{
        margin-left: 0rem;
        font-size: 17px;
    }
    .nav-link{
      color: black  !important;
    }
    .navbar-light .navbar-toggler {
    color: rgba(0, 0, 0, 0.5);
    border-color: rgba(0, 0, 0, 0.1);
    outline: none;
}
    .for{
        text-align: center;
        margin-top: 1rem;
        color: white;
    }
    .for a{
        color: white;
    }
    .form-group input{
        background: #F9F9FA  !important;
        border-radius: 8px;
        padding: 8px 8px;
        margin-bottom: 1rem;
        width: 100%;
    }
    }
</style>