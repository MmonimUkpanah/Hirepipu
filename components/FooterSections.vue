<template>
    <div class="footer">
        <footer>
            <div class="one">
                <img src="/img/logo.svg" alt="">
                <p>LaslesVPN is a private virtual network that has unique features and has high security.</p>
                <p>copyright 2020 Hirepipu. All Rights Reserved</p>
            </div>
            <div class="two">
                <h5>Company</h5>
                <p>About Us</p>
                <p>Contact Us</p>
                <p>Terms</p>
            </div>
            <div class="three">
                <h5>Product</h5>
                <p>Job Seeker</p>
                <p>Recruiter</p>
                <p>Locations</p>
            </div>
            <div class="four">
                <h5>Socials</h5>
               <img src="/img/s.svg" alt=""> <img src="/img/twi.svg" alt=""> <img src="/img/tor.svg" alt="">
            </div>
        </footer>
    </div>
</template>
<style scoped>
   .footer{
       background: #ECE7E7;
       padding-top: 2rem;
       padding-bottom: 2rem;
   }
    footer{
        margin-left: 10%;
        margin-right: 10%;
        display: grid;
        grid-template-columns: 2fr 1fr 1fr 1fr;
        grid-gap: 2rem;
    }
    .four img{
        margin-right: 0.5rem;
    }
    @media(max-width:567px){
        footer{
        margin-left: 10px;
        margin-right: 10px;
        display: grid;
        grid-template-columns: 1fr 1fr;
        text-align: center;
        grid-gap: 1rem;
    }
    }

    @media(min-width: 568px) and (max-width:768px){
        footer{
        margin-left: 10px;
        margin-right: 10px;
        display: grid;
        grid-template-columns: 2fr 1fr 1fr 1fr;
        
        grid-gap: 1rem;
    }
    }
</style>