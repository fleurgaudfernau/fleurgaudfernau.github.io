---
layout: page
permalink: /Cortical_surface_atlas_/
show-avatar: true
display_categories: [work]
---
<html>
  <head>
<style> 
.rangeslider {
  width: 400px;
  margin: 0 auto;
}
.myslider {
  -webkit-appearance: none;
  background: #FCF3CF;
  width: 100%;
  height: 20px;
  opacity: 1;
  margin-top: 100px;
  border-radius: 10px;
}
 .slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 100%;
  height: 24px;
  border: 0;
  cursor: pointer;
}
.slider::-moz-range-thumb {
  width: 95%;
  height: 25px;
  border: 0;
  cursor: pointer;
} 
.myslider:hover {
  opacity: 1;
}
.image {
  position: relative;
  width: 400px;
  margin: 0 auto;
}
.image>img {
  position: absolute;
  display: none;
}
.image>img.visible,
.image>img:first-child {
  display: block;
}
.sliderOutput>div {
  margin: 5px;
  width: 120px;
  display: inline-block;
  vertical-align: top;
  text-align: center;
}
.sliderOutput h6,
.sliderOutput p {
  margin: 5px;
}
</style> 
  </head>
<body>
<div class="rangeslider">
    <input type="range" min="20.00" max="21.00" step="0.1" value="0.1" class="myslider" 
      id="sliderRange" onchange="myFunction(this.value)" oninput="myFunction(this.value)"
      >
   <span id="myValue"></span>
</div>

<br>
<br>
<br>


<script type="text/javascript"> 
  function myFunction(val) {
    document.getElementById("myValue").innerHTML = val;
}
  // var rangeslider = document.getElementById("sliderRange"); 
   //var output = document.getElementById("demo"); 
   //output.innerHTML = rangeslider.value; 
   //rangeslider.oninput = function() { 
    //   output.innerHTML = this.value; 
  //} 
</script> 
</body>

<a href="https://kitware.github.io/itk-vtk-viewer/app/?fileToLoad=https://github.com/fleurgaudfernau/fleurgaudfernau.github.io/tree/master/assets/img/sub-sub-035_hole__filled.vtk">Visualize me in 3D online:</a>
  
  <a href="https://kitware.github.io/itk-vtk-viewer/app/?fileToLoad=https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/fleurgaudfernau/fleurgaudfernau.github.io/tree/master/assets/img/sub-sub-035_hole__filled.vtk"> 
Visualize me in 3D online:</a>

<div class="image mt-10 mb-10" id="sliderImages">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_0__age_20.00_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_1__age_20.10_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_2__age_20.20_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_3__age_20.30_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_4__age_20.40_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_5__age_20.50_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_6__age_20.60_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_7__age_20.70_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_8__age_20.80_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_9__age_20.90_smooth_300_.png">
    <img src="/assets/atlas/inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_2__tp_100__age_30.00_smooth_300_.png">  
</div>

</html>

