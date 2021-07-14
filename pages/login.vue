<template>
    <div>
        <Navbar/>
         <div class="up">
        
        <div class="up1">
            <div class="up2">
                <div class="up21">
                    <img src="/img/hpp.svg" alt="logo" srcset=""/>
                    <h1>Hirepipu</h1>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Minima voluptatum nisi omnis ut ipsam alias quasi excepturi, magni provident eos!</p>
                </div>
                
            </div>
            <div class="up3">
                <div class="up31">
                    <h1>Login</h1>
                    <form action="" method="post">
                        <label for="">Email</label>
                        <input type="email" class="form-control">
                        <label for="">Password</label>
                        <input type="password" class="form-control">
                        <button class="btn btn-primary">Login</button>
                    </form>
                </div>
                
            </div>
        </div>
    </div> 
        <footer-sections/>
    </div>
    
</template>
<style scoped>
    .up{
        background-color: #1B6AE3;
        height: 100vh;
    }
    .btn-primary{
        background-color: #1B6AE3 !important;
        margin-top: 1rem;
        width: 100%;
    }
    .up1{
        display: grid;
        grid-template-columns: 1fr 1fr;
    }
    label{
        display: block;
    }
    
    .up31{
        background: white;
        margin-top: 5.5rem;
        padding-top: 2rem;
        padding-left: 2rem;
        padding-right: 2rem;
        padding-bottom: 15rem;
        margin-right: 2rem;
        margin-left: 2rem;
        border-radius: 10px;
    }
    .up31 h1{
        color: #1B6AE3;
    }
    .up321{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 1rem;
    }
    .up21{
        margin-top: 5rem;
        margin-bottom: 5rem;
        margin-left: 2rem;
        margin-left: 2rem;
        text-align: center;
    }
    .up21 h1{
        color: white;
        font-size: 70px;
        margin-top: -7rem;
    }
    .up21 p{
        color: white;
        margin-left: 5rem;
        margin-right: 5rem;
    }
    .up2 img{
        width: 50%;
    }


    @media(max-width:567px){
        .up1{
        display: grid;
        grid-template-columns: 1fr;
    }
        .up321{
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 1rem;
    }
        .up31{
        background: white;
        margin-top: 3rem;
        padding: 3rem 2rem;
        margin-right: 10px;
        margin-left: 10px;
        border-radius: 10px;
    }
    .up21{
        margin-top: 5rem;
        margin-bottom: 5rem;
        margin-left: 10px;
        margin-left: 10px;
        text-align: center;
    }
    .up21 p{
        color: white;
        margin-left: 10px;
        margin-right: 10px;
    }
    .up2 img{
        width: 90%;
    }
    .up21 h1{
        color: white;
        font-size: 70px;
        margin-top: -3rem;
    }
    .up{
        background-color: #1B6AE3;
        height: 200vh;
    }
    input{
        margin-bottom: 0.5rem;
    }
    }


    @media(min-width:568px) and (max-width:768px){
        .up2 img{
        width: 90%;
    }
        .up321{
        display: grid;
        grid-template-columns: 1fr;
        grid-gap: 1rem;
    }
    }

    @media(min-width:769px) and (max-width:1200px){
        .up2 img{
        width: 80%;
    }
        .up31{
        background: white;
        margin-top: 3rem;
        padding: 5rem 2rem;
        margin-right: 2rem;
        margin-left: 2rem;
        border-radius: 10px;
    }
    }
</style>