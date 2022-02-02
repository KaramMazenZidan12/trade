<template>
<div class="container" id="container">

<h1 class="text-center" id="h1">Cars F-company</h1>
<br>
<br>
<ul class="nav nav-pills mb-3 justify-content-center font-weight-bold" id="pills-tab" role="tablist">
  <li class="nav-item">
    <a class="nav-link active" id="pills-home-tab" data-toggle="pill" href="#pills-home" role="tab" aria-controls="pills-home" aria-selected="true">Cars</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="pills-profile-tab" data-toggle="pill" href="#pills-profile" role="tab" aria-controls="pills-profile" aria-selected="false">Mercedes</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" id="pills-contact-tab" data-toggle="pill" href="#pills-contact" role="tab" aria-controls="pills-contact" aria-selected="false">Audi</a>
  </li>
</ul>

<div class="tab-content " id="pills-tabContent">
<center>
<span class="font-weight-bold">0 $ </span>
<input id="multi1" class="multi-range" type="range"  />
<span class="font-weight-bold"> 120000 $</span>
</center>
  <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">

  <div class="row">
  <div class="col-md-4 text-center"  v-for="c in itemsCopy" :key="c">
     <div class="card">
<!-- set a width on the image otherwise it will expand to full width       -->
      <img class="card-img-top img-fluid" :src="require('@/assets/images/'+ c.t + '.jpg')" alt="Card image cap" width="400" style="height:250px">
      <div class="card-body">
        <h3 class="card-title font-weight-bold">Car {{ c.t1 }}</h3>
            <div class="d-flex align-items-center justify-content-center colors my-2">
                                <div class="btn-group" data-toggle="buttons" data-tooltip="tooltip" data-placement="right" title="choose color">  
                                 <label class="btn btn-black form-check-label"> </label>
                                  <label class="btn btn-white form-check-label">  </label> 
                                  <label class="btn btn-gold form-check-label"> </label> </div>
                            </div>
        <p class="card-text font-weight-bold">{{ c.t2 }} <span>$</span></p>
      </div>
      <div class="card-footer font-weight-bold">
      order now 
      
      </div>
    </div>
  
  </div>
  
  
  
  </div>

 
    <!-- /.card -->


    <br>
   <nav class="mb-4 d-flex justify-content-center">
    <pagination v-model="page" :records="18" :per-page="9" @paginate="myCallback"/>
</nav>


  
  </div>

  <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">

 <div class="row">
  <div class="col-md-4 text-center"  v-for="c in itemsCopy2" :key="c">
     <div class="card">
<!-- set a width on the image otherwise it will expand to full width       -->
      <img class="card-img-top img-fluid" :src="require('@/assets/images/'+ c.t + '.jpg')" alt="Card image cap" width="400" style="height:250px">
      <div class="card-body">
        <h3 class="card-title font-weight-bold">Car {{ c.t1 }}</h3>
            <div class="d-flex align-items-center justify-content-center colors my-2">
                                <div class="btn-group" data-toggle="buttons" data-tooltip="tooltip" data-placement="right" title="choose color">  
                                 <label class="btn btn-black form-check-label"> </label>
                                  <label class="btn btn-white form-check-label">  </label> 
                                  <label class="btn btn-gold form-check-label"> </label> </div>
                            </div>
        <p class="card-text font-weight-bold">{{ c.t2 }} <span>$</span></p>
      </div>
      <div class="card-footer font-weight-bold">
      order now 
      </div>
    </div>
  
  </div>
  
  
  
  </div>

  
    <br>
   <nav class="mb-4 d-flex justify-content-center">
    <pagination v-model="page" :records="9" :per-page="6" @paginate="myCallbacks"/>
</nav>

  
  </div>

  <div class="tab-pane fade " id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">
   <div class="row">
  <div class="col-md-4 text-center"  v-for="c in itemsCopys" :key="c">
     <div class="card">
<!-- set a width on the image otherwise it will expand to full width       -->
      <img class="card-img-top img-fluid" :src="require('@/assets/images/'+ c.t + '.jpg')" alt="Card image cap" width="400" style="height:250px">
      <div class="card-body">
        <h3 class="card-title font-weight-bold">Car {{ c.t1 }}</h3>
             <div class="d-flex align-items-center justify-content-center colors my-2">
                                <div class="btn-group" data-toggle="buttons" data-tooltip="tooltip" data-placement="right" title="choose color">  
                                 <label class="btn btn-black form-check-label"> </label>
                                  <label class="btn btn-white form-check-label">  </label> 
                                  <label class="btn btn-gold form-check-label"> </label> </div>
                            </div>
        <p class="card-text font-weight-bold">{{ c.t2 }} <span>$</span></p>
     
      </div>
      <div class="card-footer font-weight-bold">
      order now 
      </div>
    </div>
  
  </div>
  


  
  </div>
   <br>
   <nav class="mb-4 d-flex justify-content-center">
    <pagination v-model="page" :records="9" :per-page="6" @paginate="myCallbackss"/>
</nav>


  </div>

</div>



</div>

</template>

<script>
import Pagination from 'v-pagination-3';
export default {

  name: 'Section3',
     components: {
    Pagination,
    },
    
data() {
  return {
   page: 1,
    
        cars: [

       { t: '1' ,t1:'78isi' ,t2:30000},
        { t: '11' ,t1:'78isi' ,t2:30000},
         { t: '2',t1:'78isi' ,t2:30000 },
          { t: '22' ,t1:'78isi' ,t2:30000},
           { t: '3',t1:'78isi' ,t2:30000 },
            { t: '33' ,t1:'78isi' ,t2:30000},
               { t: '4' ,t1:'78isi' ,t2:30000},
        { t: '44' ,t1:'78isi' ,t2:30000},
         { t: '5' ,t1:'78isi' ,t2:30000},
          { t: '55',t1:'78isi' ,t2:30000 },
           { t: '6',t1:'78isi' ,t2:30000 },
            { t: '66',t1:'78isi' ,t2:30000 },
               { t: '7',t1:'78isi' ,t2:30000 },
        { t: '77' ,t1:'78isi' ,t2:30000},
         { t: '8' ,t1:'78isi' ,t2:30000},
          { t: '88' ,t1:'78isi' ,t2:30000},
           { t: '3' ,t1:'78isi' ,t2:30000},
            { t: '99',t1:'78isi' ,t2:30000 },
    ],
       carss: [
       { t: '1' ,t1:'78isi' ,t2:30000},
               { t: '2',t1:'78isi' ,t2:30000 },
           { t: '3',t1:'78isi' ,t2:30000 },
               { t: '4' ,t1:'78isi' ,t2:30000},
         { t: '5' ,t1:'78isi' ,t2:30000},
           { t: '6',t1:'78isi' ,t2:30000 },
               { t: '7',t1:'78isi' ,t2:30000 },
         { t: '8' ,t1:'78isi' ,t2:30000},
           { t: '3' ,t1:'78isi' ,t2:30000},    
    ],
       carsss: [
         { t: '11',t1:'78isi' ,t2:30000 },
          { t: '22' ,t1:'78isi' ,t2:30000},
            { t: '33' ,t1:'78isi' ,t2:30000}, 
        { t: '44' ,t1:'78isi' ,t2:30000},
          { t: '55',t1:'78isi' ,t2:30000 },
            { t: '66',t1:'78isi' ,t2:30000 },    
        { t: '77' ,t1:'78isi' ,t2:30000},
          { t: '88' ,t1:'78isi' ,t2:30000},
            { t: '99',t1:'78isi' ,t2:30000 },
    ],
itemsCopy :[{ t: '1' ,t1:'78isi' ,t2:30000},
        { t: '11' ,t1:'78isi' ,t2:30000},
         { t: '2',t1:'78isi' ,t2:30000 },
          { t: '22' ,t1:'78isi' ,t2:30000},
           { t: '3',t1:'78isi' ,t2:30000 },
            { t: '33' ,t1:'78isi' ,t2:30000},
               { t: '4' ,t1:'78isi' ,t2:30000},
        { t: '44' ,t1:'78isi' ,t2:30000},],

        itemsCopy2:[{ t: '1' ,t1:'78isi' ,t2:30000},
               { t: '2',t1:'78isi' ,t2:30000 },
           { t: '3',t1:'78isi' ,t2:30000 },
               { t: '4' ,t1:'78isi' ,t2:30000},
         { t: '5' ,t1:'78isi' ,t2:30000},
           { t: '6',t1:'78isi' ,t2:30000 }],
           itemsCopys:[{ t: '11',t1:'78isi' ,t2:30000 },
          { t: '22' ,t1:'78isi' ,t2:30000},
            { t: '33' ,t1:'78isi' ,t2:30000}, 
        { t: '44' ,t1:'78isi' ,t2:30000},
          { t: '55',t1:'78isi' ,t2:30000 },
            { t: '66',t1:'78isi' ,t2:30000 }],
  
  }
},
methods: {
  myCallback(){
         for (var i=9; i<=18; i++) {
  this.itemsCopy = Object.assign({}, this.cars);
  }
  },
      myCallbacks(){
         for (var i=7; i<=9; i++) {
  this.itemsCopy2 = Object.assign({}, this.carss);
  }
  },
     myCallbackss(){
         for (var i=7; i<=9; i++) {
  this.itemsCopys = Object.assign({}, this.carsss);
  }
  },
},
}

</script>
<style scoped>
#h1{
font-size: 5vw;
}
.card-text  span{
color:#E7AC4E;
}

.nav-link,#container h1{
color:#E7AC4E;
}
 li{
    margin-right:0.5rem;
   }
 .card{
   margin-top:0.8rem;
      margin-right:-1rem;
    box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
 }


.card-footer{
filter: brightness(1.1);
background:#E7AC4E;
color: white;
text-shadow: 1px 1px 2px rgba(100, 100, 111, 0.2) ;
}
.card-text ,.card-title,.font-weight-bold{
   color:rgba(51, 51, 51, 0.856);
} 
.col-md-4 .card:hover,.col-md-4 .car:focus{
 box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
   border: 2px solid #E7AC4E;
   transform: scale(1,1);
}
.btn-black {
    background-color: #333;
    border-radius: 5%;
}

.btn-white {
    background-color: white;
    
      border-radius: 5%;
      
}

.btn-gold {
    background-color: #E7AC4E;
      border-radius: 5%;
}
input[type=range] {

  -webkit-appearance: none;
  margin: 10px 0;

}
input[type=range]:focus {
  outline: none;
}
input[type=range]::-webkit-slider-runnable-track {
  width: 100%;
  height: 10px;
  cursor: pointer;
  animate: 0.2s;
  box-shadow: 1px 1px 1px #000000;
  background: #333;
  border-radius: 5px;
  border: 1px solid #000000;
}
input[type=range]::-webkit-slider-thumb {
  box-shadow: 1px 1px 1px #000000;
  border: 1px solid #000000;
  height: 30px;
  width: 15px;
  border-radius: 5px;
  background: #E7AC4E;
  cursor: pointer;
  -webkit-appearance: none;
  margin-top: -11px;
}
</style>