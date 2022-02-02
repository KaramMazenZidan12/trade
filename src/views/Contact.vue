<template>
  <div class="container contact text-capitalize">

<div class="row" id="contatti">
<div class="container mt-5" >

    <div class="row" style="height:550px;">
      <div class="col-md-6 maps" >
         <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3220.1526220930723!2d44.0284747855496!3d36.18716988007944!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4007225537fbb40f%3A0x43fcdfdb26f55c67!2z2abZoNiMINin2LHYqNmK2YQ!5e0!3m2!1sar!2siq!4v1635586582163!5m2!1sar!2siq" frameborder="0" style="border:0" allowfullscreen></iframe>
      
      </div>
      <div class="col-md-6">
        <h2 class="text-uppercase mt-3 font-weight-bold text-white">Contact</h2>
        <form action="">
          <div class="row">
            <div class="col-lg-6">
              <div class="form-group">
                <input type="text" class="form-control mt-2" placeholder="Name" required>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="form-group">
                <input type="text" class="form-control mt-2" placeholder="Problem" required>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="form-group">
                <input type="email" class="form-control mt-2" placeholder="Email" required>
              </div>
            </div>
            <div class="col-lg-6">
              <div class="form-group">
                <input type="number" class="form-control mt-2" placeholder="Mobile" required>
              </div>
            </div>
            <div class="col-12">
              <div class="form-group">
                <textarea class="form-control" id="exampleFormControlTextarea1" placeholder="Description of the problem" rows="3" required></textarea>
              </div>
            </div>
            <div class="col-12">
            <div class="form-group">
              <div class="form-check">
                <input class="form-check-input" type="checkbox" value="" id="invalidCheck2" required>
                <label class="form-check-label" for="invalidCheck2">
                 Are you sure of the entered data?
                </label>
              </div>
            </div>
            </div>
            <div class="col-12">
              <button class="btn btn-light" type="submit">Submit</button>
            </div>
          </div>
        </form>
        <div class="text-white">
        <h2 class="text-uppercase mt-4 font-weight-bold">TEL : </h2>

        <i class="fas fa-phone mt-3"></i> <a href="tel:+">(+964) 7518406467</a><br>
        <i class="fas fa-phone mt-3"></i> <a href="tel:+">(+964) 7518406467</a><br>
        <i class="fa fa-envelope mt-3"></i> <a href="">info@test.it</a><br>
        <i class="fas fa-globe mt-3"></i> Erbil 60 Street, 1, 00184 Iraq<br>
        <i class="fas fa-globe mt-3"></i> Erbil 60 Street, 1, 00184 Iraq<br>
      
        </div>
      </div>

    </div>
</div>
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
  name: 'Contact',
  components: {
    Footer,
    Section4,
  },
}
</script>
<style scoped>
.contact{
border : 2px solid #ffcb78;
border-right: none;
border-left: none;
}
#contatti{
  background-color: #333;
  letter-spacing: 2px;
  }
#contatti a{
  color: #fff;
  text-decoration: none;
}


@media (max-width: 575.98px) {

  #contatti{padding-bottom: 800px;}
  #contatti .maps iframe{
    width: 100%;
    height: 450px;
  }
 }


@media (min-width: 576px) {

   #contatti{padding-bottom: 800px;}

   #contatti .maps iframe{
     width: 100%;
     height: 450px;
   }
 }

@media (min-width: 768px) {

  #contatti{padding-bottom: 350px;}

  #contatti .maps iframe{
    width: 100%;
    height: 850px;
  }
}

@media (min-width: 992px) {
  #contatti{padding-bottom: 200px;}

   #contatti .maps iframe{
     width: 100%;
     height: 700px;
   }
}


#author a{
  color: #fff;
  text-decoration: none;
    
}
.fas,.fa{
color:#ffcb78;

}
.btn{

    background:#ffcb78;
    color: #fff;
    border-color:#ffcb78 ;
}
</style>