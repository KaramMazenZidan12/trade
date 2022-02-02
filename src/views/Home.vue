<template>
 <div class="container text-capitalize" id="containers">
<Section1/>
<br>
<Section2/>
<br>
<br>
<Section3/>
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
import Section1 from '@/components/Section1.vue'
import Section2 from '@/components/Section2.vue'
import Section3 from '@/components/Section3.vue'
import Section4 from '@/components/Section4.vue'
export default {
  name: 'App',
  components: {
    Footer,
    Section1,
    Section2,
    Section3,
    Section4,
  },
}
</script>
<style scoped>
#containers{
border : 2px solid #ffcb78;
border-right: none;
border-left: none;
border-top: none;
}
</style>