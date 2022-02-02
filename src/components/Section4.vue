<template>
<div class="container" >
<h1 class="responser text-center ">Responser</h1>
 <br>
 
 <carousel :items-to-show="3" :autoplay="3000" >
  
    <slide v-for="slide in itemss" :key="slide" >
       <img class="res" :src="require('@/assets/responser/'+ slide.v + '.png')" alt="Card image cap"  >
    </slide>
    <template #addons>
      <navigation />
   
    </template>
  </carousel>

<br> <br>

</div>

</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide,  Navigation } from 'vue3-carousel';
export default {
 name: 'Section4',
 components: {
    Carousel,
    Slide,
    Navigation,},
  
   data() {
  return {
               itemss: [
       { v: '1' },
        { v: '2' },
         { v: '3' },
          { v: '1' },
           { v: '2' },
            { v: '3' },
    ],
  }
},
}

</script>
<style scoped>
.responser{
color:#E7AC4E;
font-size: 6vw;
}
.res{
width: 140px;
}
@media only screen and (max-width: 1024px) {
.res{
width:80px;
}
}
@media only screen and (max-width: 765px) {
.res{
width: 50px;
}
}
@media only screen and (max-width: 465px) {
.res{
width: 35px;
}
}
</style>