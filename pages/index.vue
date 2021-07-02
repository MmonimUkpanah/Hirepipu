<template>
  <div>
    <Navbar />
    <div class="in">
      <div class="in1">
        <h1>Get easy access to jobs and post jobs</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Doloremque corrupti minima nam recusandae. Molestias tempora atque animi quis quaerat delectus culpa veniam adipisci ipsum. Quibusdam laborum quae officia minima architecto.</p>
        <button>Get Started</button>
      </div>
      <div class="in2">
        <img src="/img/pips.svg" alt="logo" srcset=""/>
      </div>
    </div>
      <div class="job">
      <div class="job1 bo " >
        <img src="/img/1.svg" alt="logo" srcset=""/>
        <div>
          <h3>1000+</h3>
          <p>Jobs</p>
        </div>
      </div>
      <div class="job1 bo">
        <img src="/img/2.svg" alt="logo" srcset=""/>
        <div>
          <h3>30+</h3>
          <p>Locations</p>
        </div>
      </div>
      <div class="job1" >
        <img src="/img/3.svg" alt="logo" srcset=""/>
        <div>
          <h3>200+</h3>
          <p>Placements</p>
        </div>
      </div>
    </div>
      <div class="fe">
      <div class="fe1">
        <div class="fe2">
          <img src="/img/pips.svg" alt="logo" srcset=""/>
        </div>
        <div class="fe3">
          <h3>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Odit quas nobis laboriosam eius!</h3>
          <p>You can explore the features that we provide.</p>
          <div class="fe31">
            <p><img src="/img/34.svg" alt="logo" srcset=""/> Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
            <p><img src="/img/34.svg" alt="logo" srcset=""/> Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
            <p><img src="/img/34.svg" alt="logo" srcset=""/> Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
            <p><img src="/img/34.svg" alt="logo" srcset=""/> Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
            <p><img src="/img/34.svg" alt="logo" srcset=""/> Lorem ipsum dolor sit, amet consectetur adipisicing.</p>
          </div>
        </div>
      </div>
    </div> 
     <div class="lo">
      <div class="lo1">
        <div class="lo2">
          <img src="/img/ps.svg" alt="">
        </div>
        <div class="lo3">
          <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit. At in molestias optio porro saepe hic.</h3>
        </div>
        
      </div>
      <div class="lo4">
        <input type="text" placeholder="Enter Email Address"><button>Subscribe</button>
      </div>
    </div> 
     <div class="te">
      <div class="te1">
        <h3>Testimonies</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quis, expedita.</p>
      </div>
      <div class="te2">
        <div class="te21">
          <div class="te211">
            <img src="/img/4.svg" alt="">
            <div class="te2112">
              <h5>Triple H</h5>
              <p>Port Harcourt</p>
            </div>
            
              <span>4.5 <img src="/img/h.svg" alt=""></span>
          
          </div>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Tristique nulla vestibulum, pretium, diam dui, tempor, auctor eget morbi. </p>
        </div>
        <div class="te22">
          <div class="te211">
            <img src="/img/4.svg" alt="">
            <div class="te2112">
              <h5>Triple H</h5>
              <p>Port Harcourt</p>
            </div>
            
              <span>4.5 <img src="/img/h.svg" alt=""></span>
          
          </div>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae atque ipsam possimus porro debitis consequuntur quidem modi dolorem libero repellendus.</p>
        </div>
        <div class="te21">
          <div class="te211">
            <img src="/img/4.svg" alt="">
            <div class="te2112">
              <h5>Triple H</h5>
              <p>Port Harcourt</p>
            </div>
            
              <span>4.5 <img src="/img/h.svg" alt=""></span>
          
          </div>
          <p>“This is very unusual for my business that currently requires a virtual private network that has high security.”.</p>
        </div>
       
      </div>
        <div class="te3">
          <img src="/img/l.svg" alt=""><img src="/img/r.svg" alt="">
        </div> 
    
    </div> 
  <footer-sections/>
    
  </div>
</template>


<style scoped>
  .in{
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-left: 10%;
    margin-right: 10%;
    margin-top: 2rem;
  }
  
  .in1 h1{
    font-size: 50px;
    color: #0B132A;
  }
  .in1 p{
    color: #4F5665;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }
  .in1 button{
    background-color:#1B6AE3 ;
    padding: 5px 30px;
    color: white;
    border-radius: 50px;
    border: none;
  }
  .in2{
    text-align: center;
  }
  .job{
    margin-left: 15%;
    margin-right: 15%;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    text-align: center;
    margin-top: 3rem;
    border-radius: 10px !important;
    background: white;
    z-index: 1;
  }
  .job1{
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding-left: 6rem;
    padding-right: 6rem;
    background: white;
    z-index: 1;
    
  }
  
  .job1 h3{
    color: #0B132A;
    font-weight: 700;
  }
  .job1 p{
    color: #4F5665;
  }
  .job1 img{
    width: 4rem;
  }
  .bo{
    border-right: 2px solid #EEEFF2;
  }
  .fe{
    background-color: #1B6AE3;
    margin-top: -3rem;
    z-index: -1;
  }
  .fe1{
    padding-top: 5rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-right: 10%;
    margin-left: 10%;
  }
  .fe2{
    text-align: center;
  }
  .fe3{
    color: white;
  }
  .fe3 p{
    margin-top: 1rem;
  }
  .lo{
    background: url("/img/ba.svg") no-repeat center center/cover;
    padding-top: 6rem;
    padding-bottom: 6rem;
  }
  .lo1{
    
    margin-left: 10%;
    margin-right: 10%;
    background: white;
    border-radius: 10px;
    display: grid;
    padding: 2rem 5rem;
    grid-template-columns: 1fr 1fr;
  }
  .lo2{
    text-align: center;
  }
  .lo3{
    padding-top: 5rem;
    padding-bottom: 5rem;
    font-weight: 500;
  }
  .lo4{
    margin-left: 10%;
    margin-right: 10%;
    margin-top: 0.5rem;
  }
  .lo4 input{
    width: 60%;
    height: 40px;
    margin-right: 0.5rem;
    border: none;
    padding-left: 1rem;
    border-radius: 5px;
  }
  .lo4 button{
    width: 39%;
    height: 40px;
    border: none;
    border-radius: 5px;
  }
  .te{
    margin-top: 2rem;
    margin-left: 5%;
    margin-right: 5%;
  }
  .te1{
    text-align: center;
  }
  .te1 h3{
    font-weight: 500;
  }
  .te2{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-column-gap: 2rem;
  }
  .te21{
    border: 2px solid #1B6AE3;
    border-radius: 10px;
    padding: 3rem 4rem;
  }
  .te22{
    border: 2px solid #FFBF1A;
    border-radius: 10px;
    padding: 2rem 2rem;
  }
  .te211{
    display: grid;
    grid-template-columns: 1fr 3fr 1fr;
  }
  .te3{
    text-align: center;
    margin-top: 2rem;
    margin-bottom: 2rem;
    
  }
  .te3 img{
    margin-right: 0.5rem;
    margin-left: 0.5rem;
  }







  @media(max-width:567px){
    
    .in{
    display: grid;
    grid-template-columns: 1fr;
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
    text-align: center;
  }
  .in1{
    margin-bottom: 2rem;
  }
  .in2 img{
    width: 100%;
  }
  .job{
    margin-left: 10px;
    margin-right: 10px;
    display: grid;
    grid-template-columns: 1fr;
    text-align: center;
    margin-top: 3rem;
    border-radius: 10px;
  }
   .job1{
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding-left: 3rem;
    padding-right: 3rem;
  }
  .job1 img{
    width: 3rem;
  }
  .fe{
    background-color: #1B6AE3;
    margin-top: -3rem;
    z-index: -1;
  }
  .fe1{
    padding-top: 5rem;
    display: grid;
    grid-template-columns: 1fr;
    margin-right: 0px;
    margin-left: 0px;
    width: 100%;
  }
  .fe2{
    text-align: center;
    width: 100%;
  }
  .fe2 img{
    width: 90%;
  }
  .fe3{
    color: white;
    text-align: center;
    margin-left: 10px;
    margin-right: 10px;
  }
  .fe3 p{
    margin-top: 1rem;
  }
  .lo{
    background: url("/img/ba.svg") no-repeat center center/cover;
    padding-top: 6rem;
    padding-bottom: 6rem;
  }
  .lo1{
    
    margin-left: 10px;
    margin-right: 10px;
    background: white;
    border-radius: 10px;
    display: grid;
    padding: 2rem 10px;
    text-align: center;
    grid-template-columns: 1fr;
  }
  .lo2{
    text-align: center;
  }
  .lo2 img{
    width: 100%;
  }
  .lo3{
    padding-top: 5rem;
    padding-bottom: 5rem;
    font-weight: 500;
  }
  .lo4{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 0.5rem;
  }
  .lo4 input{
    width: 57%;
    height: 40px;
    margin-right: 0.5rem;
    border: none;
    border-radius: 5px;
  }
  .lo4 button{
    width: 40%;
    height: 40px;
    border: none;
    border-radius: 5px;
  }
  .te{
    margin-top: 2rem;
    margin-left: 10px;
    margin-right: 10px;
  }
  .te1{
    text-align: center;
  }
  .te1 h3{
    font-weight: 500;
  }
  .te2{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    grid-row-gap: 2rem;
  }
  .te21{
    border: 2px solid #1B6AE3;
    border-radius: 10px;
    padding: 3rem 1rem;
  }
  .te22{
    border: 2px solid #FFBF1A;
    border-radius: 10px;
    padding: 2rem 2rem;
  }
  .te211{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  .te3{
    text-align: center;
    margin-top: 2rem;
    
  }
  .te3 img{
    margin-right: 0.5rem;
    margin-left: 0.5rem;
  }

  }


  @media(min-width: 568px) and (max-width:768px){
     .job{
    margin-left: 15px;
    margin-right: 15px;
    display: grid;
    grid-template-columns: 1fr ;
    text-align: center;
    margin-top: 3rem;
    border-radius: 10px !important;
    background: white;
    z-index: 1;
  }
  .te2{
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    grid-row-gap: 2rem;
  }
   .job1{
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding-left: 16rem;
    padding-right: 16rem;
    background: white;
    z-index: 1;
    
  }
  .in{
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 2rem;
  }
    .fe1{
    padding-top: 5rem;
    display: grid;
    grid-template-columns: 1fr 1fr;
    margin-right: 10px;
    margin-left: 10px;
  }
   .lo1{
    
    margin-left: 10px;
    margin-right: 10px;
    background: white;
    border-radius: 10px;
    display: grid;
    padding: 2rem 5rem;
    grid-template-columns: 1fr 1fr;
  }
  .lo4{
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 0.5rem;
  }
  .lo4 input{
    width: 57%;
    height: 40px;
    margin-right: 0.5rem;
    border: none;
    border-radius: 5px;
  }
  .lo4 button{
    width: 40%;
    height: 40px;
    border: none;
    border-radius: 5px;
  }
  }


  @media(min-width: 769px) and (max-width:1200px){
    .job{
    margin-left:0;
    margin-right: 0;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr ;
    text-align: center;
    margin-top: 3rem;
    border-radius: 10px !important;
    background: white;
    z-index: 1;
  }
  }
</style>




