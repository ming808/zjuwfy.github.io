---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


<html>
  <head>
    <style>
      .slideshow-container {
        max-width: 1000px;
        position: relative;
        margin: auto;
        overflow: hidden;
      }
      
      .mySlides {
        display: none;
      }
      
      .prev, .next {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: auto;
        margin-top: -22px;
        padding: 16px;
        color: white;
        font-weight: bold;
        font-size: 18px;
        transition: 0.6s ease;
        border-radius: 0 3px 3px 0;
        user-select: none;
      }
      
      .next {
        right: 0;
        border-radius: 3px 0 0 3px;
      }
      
      .prev:hover, .next:hover {
        background-color: rgba(0,0,0,0.8);
      }
    </style>
  </head>
  <body>
    <div class="slideshow-container">
      <div class="mySlides">
        <img src="/images/image4.jpg" style="width:100%">
      </div>
      <div class="mySlides">
        <img src="/images/image5.jpg" style="width:100%">
      </div>
      <div class="mySlides">
        <img src="/images/image6.jpg" style="width:100%">
      </div>
      <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
      <a class="next" onclick="plusSlides(1)">&#10095;</a>
    </div>
    <script>
      var slideIndex = 1;
      showSlides(slideIndex);
      
      function plusSlides(n) {
        showSlides(slideIndex += n);
      }
      
      function showSlides(n) {
        var i;
        var slides = document.getElementsByClassName("mySlides");
        if (n > slides.length) {slideIndex = 1}
        if (n < 1) {slideIndex = slides.length}
        for (i = 0; i < slides.length; i++) {
            slides[i].style.display = "none";
        }
        slides[slideIndex-1].style.display = "block";
      }
    </script>
  </body>
</html>
