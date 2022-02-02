<template>

 <div class="container px-lg-5">
  <div class="row mx-lg-n5">
    <div class="col-md-4 py-3 px-lg-5 col-sm-12 text-center" id="icons">
    
  <i class="fab fa-slack"></i>
  
    <p><br>Car wash in a sophisticated and modern style, using the best types of cleaning tools</p>
    
    </div>
    <div class="col-md-4  py-3 px-lg-5  col-sm-12 text-center" id="icons">
    <i class="fas fa-car-crash"></i>
    
    <p><br>Repairing all car parts under the supervision of international expertise and international equipment and using original parts</p>
    </div>

    <div class="col-md-4  py-3 px-lg-5  col-sm-12 text-center" id="icons">
 <i class="fas fa-exchange-alt"></i>
 <br>
    <p><br>You can change your old car and get a new car with a small payment</p>
    </div>
  </div>
</div>


</template>

<script>

export default {

  name: 'Section2',
   
}

</script>
<style scoped>


.fab ,.fas{
font-size:5vw;
color:#E7AC4E;
}
.fab:hover ,.fas:hover{
 transform: rotate(45deg); 
   color:#333;
}
#icons:hover{
 box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
   border: 2px solid #E7AC4E;
}
@media only screen and (max-width: 765px) {
 .fab ,.fas{
font-size:9vw;
}
}
</style>