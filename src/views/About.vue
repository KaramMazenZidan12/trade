<template>
  <div class="container about text-capitalize">


<div class="container" id="tt" >
<br>

  <div class="row">
    <div class="col-lg-5 col-md-12 col-sm-12 ">
	<center>
<img  class="aboutimage" src="../assets/images/logo.png" >
</center>
</div>

	

    <div class="col-lg-7 col-md-12 col-sm-12">    
	<h3>What does this company do ??</h3>
	<p> A company specializing in the sale of cars and car parts of two types only Mercedes and Audi .</p>
	
	<h3>What services does this company provide in the event of any car malfunction ??</h3>
	<p>This company provides all original spare parts with the latest tools and under the supervision of the best engineers.</p>
	
	<h3>Are there other services ??</h3>
	<p>There is a car wash and an oil change under the supervision of specialists and the latest tools </p>
	
	<h3>Can I sell my old car ??</h3>
	<p>Yes, and you can exchange the old car for a new one by paying a small amount .</p>
	
	
  </div>
  
</div>
<br>
</div>
 
 <br>
<br>
<Section4/>
<br>
<br>
<Footer/>
  </div>
</template>

<script>
import Footer from '@/components/Footer.vue'
import Section4 from '@/components/Section4.vue'
export default {
  name: 'App',
  components: {
    Footer,
    Section4,
  },
}
</script>
<style scoped>
.about{
border : 2px solid #ffcb78;
border-right: none;
border-left: none;
}

h3,p{
color:#333;
}
.aboutimage{
width:100%;
}
@media only screen and (max-width: 768px) {
.aboutimage{
width:60%;
}
}
</style>