<template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-light ">
      <div class="nav1">
        <div class="container-fluid">
        <a class="navbar-brand" href="#"><img src="/img/logo.svg" alt="logo" srcset=""/></a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarTogglerDemo02" aria-controls="navbarTogglerDemo02" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarTogglerDemo02">
          <ul class="navbar-nav  mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">About</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Job Seekers</a>
            </li>
           <li class="nav-item">
              <a class="nav-link" href="#">Post Jobs</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Contact Us</a>
            </li>
          </ul>
          <form >
            <span>Sign In</span>
            <button class="btn btn-outline-primary" type="submit">Register</button>
          </form>
        </div>
      </div>
      </div>
      
    </nav>
  </div>
</template>
<style scoped>
.navbar{
  display: inline !important;
}
  .nav1{
    margin-left: 10%;
    margin-right: 10%;
  }
  ul{
    margin-left: 25%;
  }
  li a{
    color: #1B6AE3 !important;
    margin-left: 1rem;
  }
  form{
    margin-left: auto;
  }
  form span{
    color: #1B6AE3 !important;
  }
  form button{
    background-color: #1B6AE3;
    color: white;
    margin-left: 1rem;
    border-radius: 50px;
  }
  .navbar-light .navbar-toggler {
    color: rgba(0, 0, 0, 0.5);
    border-color: rgba(0, 0, 0, 0.1);
    outline-color:#1B6AE3 ;
}


  @media(max-width:768px){
    .nav1{
    margin-left:10px;
    margin-right: 10px;
  }
  ul{
    margin-left: 0;
  }
  li a{
    color: #1B6AE3 !important;
    margin-left: 0;
  }
  }
  @media (min-width: 769px) and (max-width:1200px){
     ul{
    margin-left: 5%;
  }
  }

</style>