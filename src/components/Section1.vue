<template>

 <div class="container">
 <br>
  <carousel :items-to-show="0.8" :autoplay="5000" >
  
    <slide v-for="slide in items" :key="slide" >
 
     <video class="position-relative w-100"  autoplay muted loop="-1" >
  <source :src="require('@/assets/videos/'+ slide.v + '.mp4')" type="video/mp4">
 
</video>
<h1 class="position-absolute"><span>[[ </span>Welcome In F-car <span> ]]</span><br>
German car world Just in <span>F-Company</span>
 </h1>

    </slide>
    <template #addons>
      <navigation />
   
    </template>
  </carousel>
  <br><br>
 
</div>

</template>

<script>
import 'vue3-carousel/dist/carousel.css';
import { Carousel, Slide,  Navigation } from 'vue3-carousel';
export default {

  name: 'Section1',
    components: {
    Carousel,
    Slide,
    Navigation,
    
  },
data() {
  return {
  
      items: [

       { v: '2' },
        { v: '1' },
         { v: '3' },
          { v: '4' },
           { v: '5' },
            { v: '6' },
    ],
}

}
}

</script>
<style scoped>
.container{
border-width: 2px;
border-top-color: #ffcb78;
border-top-style: solid;
}
video {
filter: brightness(0.6);
border : 2px solid #ffcb78;
}
h1{
color:white;
font-size:4vw;
text-shadow: 1px 1px 2px rgba(100, 100, 111, 0.2) ;
}
h1 span{
color:#E7AC4E;
}
</style>