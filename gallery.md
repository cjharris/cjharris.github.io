---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Gallery
permalink: /gallery/
---

<head>
  <link rel="stylesheet" type="text/css" href="/gallery.css">
</head>

<div class="container">

  <h2 style="text-align: center; color: #4f4f4f;">Mike Svob</h2>

  <div class="mySlides">
    <div class="numbertext">1 / 9</div>
    <img src="/gallery/MikeSvob.ApproachingMist.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">2 / 9</div>
    <img src="/gallery/MikeSvob.CascadeAtShannonFalls.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">3 / 9</div>
    <img src="/gallery/MikeSvob.ChestermanBeach.jpg" style="width:100%">
  </div>
    
  <div class="mySlides">
    <div class="numbertext">4 / 9</div>
    <img src="/gallery/MikeSvob.FallsAtLakeOHara.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">5 / 9</div>
    <img src="/gallery/MikeSvob.KootenayCrossing.jpg" style="width:100%">
  </div>
    
  <div class="mySlides">
    <div class="numbertext">6 / 9</div>
    <img src="/gallery/MikeSvob.LastLightVancouverIsland.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">7 / 9</div>
    <img src="/gallery/MikeSvob.LoneFir.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">8 / 9</div>
    <img src="/gallery/MikeSvob.RoadBack.jpg" style="width:100%">
  </div>

  <div class="mySlides">
    <div class="numbertext">9 / 9</div>
    <img src="/gallery/MikeSvob.SpringReflections.jpg" style="width:100%">
  </div>

  <a class="prev" onclick="plusSlides(-1)">❮</a>
  <a class="next" onclick="plusSlides(1)">❯</a>

  <div class="caption-container">
    <p id="caption"></p>
  </div>

  <div class="row">
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.ApproachingMist.jpg" style="width:100%" onclick="currentSlide(1)" alt="Approaching Mist">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.CascadeAtShannonFalls.jpg" style="width:100%" onclick="currentSlide(2)" alt="Cascade at Shannon Falls">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.ChestermanBeach.jpg" style="width:100%" onclick="currentSlide(3)" alt="Chesterman Beach">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.FallsAtLakeOHara.jpg" style="width:100%" onclick="currentSlide(4)" alt="Falls at Lake O'Hara">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.KootenayCrossing.jpg" style="width:100%" onclick="currentSlide(5)" alt="Kootenay Crossing">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.LastLightVancouverIsland.jpg" style="width:100%" onclick="currentSlide(6)" alt="Last Light Vancouver Island">
    </div>
  </div>

  <div class="row">
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.LoneFir.jpg" style="width:100%" onclick="currentSlide(7)" alt="Lone Fir">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.RoadBack.jpg" style="width:100%" onclick="currentSlide(8)" alt="Road Back">
    </div>
    <div class="column">
      <img class="demo cursor" src="/gallery/MikeSvob.SpringReflections.jpg" style="width:100%" onclick="currentSlide(9)" alt="Spring Reflections">
    </div>
  </div>  
  
</div>

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  var captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>
