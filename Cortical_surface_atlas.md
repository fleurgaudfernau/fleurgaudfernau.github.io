---
layout: page
permalink: /Cortical_surface_atlas/
show-avatar: true
display_categories: [work]
---

### style means css part
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
.slidecontainer {
  width: 100%;
}

.slider {
  -webkit-appearance: none;
  width: 80%;
  height: 25px;
  background: #d3d3d3;
  outline: none;
  opacity: 0.7;
  -webkit-transition: .2s;
  transition: opacity .2s;
}

.slider:hover {
  opacity: 1;
}

.slider::-webkit-slider-thumb {
  -webkit-appearance: none;
  appearance: none;
  width: 25px;
  height: 25px;
  background: #04AA6D;
  cursor: pointer;
}

.slider::-moz-range-thumb {
  width: 25px;
  height: 25px;
  background: #04AA6D;
  cursor: pointer;
}

.slider input[type="range"] {
-webkit-appearance:none !important;
width: 70%;
height: 2px;
background: black;
border: none;
outline: none;
}
.slider input[type="range"]::-webkit-slider-thumb {
-webkit-appearance: none !important;
width: 30px;
height:30px;
background: black;
border: 2px solid black;
border-radius: 50%;
cursor: pointer;
}
.slider input[type="range"]::-webkit-slider-thumb:hover {
background: black;
}

section {
  text-align: center;
}
figure {
  margin: 0;
}
h2 {
  position: absolute;
  color: white;
  font-size: 5em;
  font-family: sans-serif;
/*   bottom: 0; */
/*   right: 40%; */
}

section > figure {
  position: absolute;
  height: 90vh;
  display: flex;
  width: 100vw;
  justify-content: center;
}

section > figure > img {
  height: inherit;
}

section > figure {
  opacity: 0;
}

input {
  width: 20vw;
}
</style>
</head>
<body>

<h1>Custom Range Slider</h1>
<p>Drag the slider to display the current value.</p>

<div class="slidecontainer">
<input type="range" min="20.0" max="36.0" value="160" class="slider" id="myRange">
<p>Value: <span id="demo"></span></p>
</div>

<script>
var slider = document.getElementById("myRange");
var output = document.getElementById("demo");
output.innerHTML = slider.value;

slider.oninput = function() {
output.innerHTML = this.value;}

  // Display the image based on 
var src = "assets/img/atlas/Inner_cortical_surface/GeodesicRegression__GeodesicFlow__img__component_0__tp_0__age_"+ slider.value +"0_smooth_300_.png";
img = document.createElement('img');
document.getElementById("demo").innerHTML = src; 
img.src = src;
var numb = document.createElement('h2');
var fig = document.createElement('figure');
fig.appendChild(img);
fig.appendChild(numb);
document.querySelector('section').appendChild(fig); 
</script>

</body>

### another slider

<section class="timemachine">
<form action="">
 <input type="range" min="1" max="100" value="50" class="slider" id="myRange">
</form>
</section>

<script>
var images;
function jsonFlickrApi(data) {
  console.log(data);
  images = data.photos.photo.map(function(photo){return photo.url_z});
  image_elements = images.map(function(mg, i) {
    var img = document.createElement('img'); // create img
    img.src = mg; // create img path
    var numb = document.createElement('h2');
    var fig = document.createElement('figure');
    fig.appendChild(img);
    fig.appendChild(numb);
    document.querySelector('section').appendChild(fig); 
    return fig;
  });
  var slider = document.querySelector('input');
  slider.min = 0;
  slider.max = slider.value = images.length - 1;
  image_elements[slider.max].style.opacity = 1;
  // slider.step = 0.01;
  slider.addEventListener('input', function(e) {
    image_elements.forEach(function(e){e.style.opacity=0; // e.style.zIndex=-100;
                                      });
    image_elements[Math.floor(e.target.value)].style.opacity = 1;
    // image_elements[Math.floor(e.target.value)].style.zIndex=100;
}); 
}
</script>

<script>
  

</script>


<script src="https://api.flickr.com/services/rest/?method=flickr.people.getPublicPhotos&api_key=603db98e0031fb25a3e3a6fc44502683&user_id=25053835@N03&per_page=50&format=json&extras=description,license,date_upload,date_taken,owner_name,icon_server,original_format,last_update,geo,tags,machine_tags,o_dims,views,media,path_alias,url_sq,url_t,url_s,url_q,url_m,url_n,url_z,url_c,url_l,url_o">
</script>
</html>




























