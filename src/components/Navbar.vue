<template>
<div class="container">
<nav class="navbar navbar-expand-lg text-capitalize ">
  <a class="navbar-brand " href="#"><img  src="../assets/images/logo.png" width="60" height="60"></a>
<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="" role="button" ><i class="fa fa-bars" aria-hidden="true" style="color:#E7AC4E"></i></span>
</button>
  

  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto  font-weight-bold" >
      <li class="nav-item active">
        <a class="nav-link " href="#">
           <router-link to="/">home</router-link> 
        <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#"><router-link to="/about">About</router-link></a>
      </li>
       <li class="nav-item">
        <a class="nav-link " href="#"><router-link to="/contact">Contact</router-link></a>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
        <router-link to="/about">language</router-link>
        </a>
        <div class="dropdown-menu border-0" aria-labelledby="navbarDropdown">
          <a class="dropdown-item" href="#">EN</a>
          <a class="dropdown-item" href="#">AR</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item" href="#">Something Else Here</a>
        </div>
      </li>
     
    </ul>
   
 <ul class="nav navbar-nav navbar-right">



   <li class="nav-item" >
        <a class="nav-link" href="#" id="Login" >
        <i class="fas fa-sign-in-alt"></i><router-link to="/login">Login</router-link>   
    </a>
      </li>


    </ul>
  </div>
</nav>
  </div>

</template>

<script>
export default {
  name: 'Navbar',
}
</script>
<style scoped>

.navbar-toggler:focus{
    border: none;
    background: none;
}
a,.dropdown-item{
    color:#E7AC4E;
}
a:hover,.dropdown-item:hover,.fas,a:focus,.dropdown-item:focus{
    text-decoration: none;
    color:#333;
}
</style>