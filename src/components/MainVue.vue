<script  >
// document.addEventListener('test', function(){
//   var stream = document.querySelector('.slide')
//   var items = document.querySelector('.slide-active')
//   stream.addEventListener('click', function() {
//     stream.insertBefore(items[items.length - 1], items[0]);
//     items = document.querySelectorAll('.slide-active');
//   });

//   next.addEventListener('click', function() {
//     stream.appendChild(items[0]);
//     items = document.querySelectorAll('.slide-active');
//   });
// });
document.addEventListener('DOMContentLoaded', function() {
  var stream = document.querySelector('.slide');
  var items = document.querySelectorAll('.slide-img');
  var prev = document.querySelector('.slide-prev');
  var next = document.querySelector('.slide-next');

  prev.addEventListener('click', function() {
    stream.insertBefore(items[items.length - 1], items[0]);
    items = document.querySelectorAll('.slide-img');
  });

  next.addEventListener('click', function() {
    stream.appendChild(items[0]);
    items = document.querySelectorAll('.slide-img');
  });



});
</script>

<template>
    <!-- <ul class="slide-list">
      <li class="slide">
        <input type="radio" id="slide1" name="slide" >
        <label for="slide1"></label>
        <img src="../assets/image/teste.jfif" alt="">
      </li>
      <li class="slide">
        <input type="radio" id="slide2" name="slide" >
        <label for="slide2"></label>
        <img src="../assets/image/teste2.jfif" alt="">
      </li>
      <li class="slide">
        <input type="radio" id="slide3" name="slide" >
        <label for="slide3"></label>
        <img src="../assets/image/teste3.jfif" alt="">
      </li>
      <li class="slide">
        <input type="radio" id="slide4" name="slide" >
        <label for="slide4"></label>
        <img src="../assets/image/teste4.jfif" alt="">
      </li>
      
    </ul> -->
  <div class="slide-list">
  <div class="slide-prev"><img src="../assets/icons/arrow-left.svg" alt=""></div>
  <div class="slide-next"><img src="../assets/icons/arrow-right.svg" alt=""></div>
    <div class="slide">
    <li class="slide-img">
      <input type="radio" id="slide1" name="slide" checked>
      <label for="slide1"></label>
      <img src="../assets/image/teste.jfif" alt="">
    </li>
    <li class="slide-img">
      <input type="radio" id="slide2" name="slide" checked>
      <label for="slide2"></label> 
      <img src="../assets/image/teste2.jfif" alt="">
    </li>
    <li class="slide-img">
      <input type="radio" id="slide3" name="slide" checked>
      <label for="slide3"></label>
      <img src="../assets/image/teste3.jfif" alt="">
    </li>
    <li class="slide-img">
      <input type="radio" id="slide4" name="slide" checked>
      <label for="slide4"></label> 
      <img src="../assets/image/teste4.jfif" alt="">
    </li>
    </div>
</div>
</template>

<style>
/*  
.slide-list li img {
  width: 100%;
  height: 100%;
  vertical-align: top;
  margin: auto;
  position: absolute;
  
}

*/
/* .slide-list input{
  display: none;
}
.slide-list label {
  background-color: #CB954F ;
  border-radius: 50%;
  bottom: 10px;
  cursor: pointer;
  display: block;
  height: 10px;
  position: absolute;
  width: 10px;
  z-index: 10;
}
 */

  
  /* .gallery {
  position: absolute;
  top: 50%;
  width: 100%;
  height: 90%;
  max-height: 28vw;
  transform: translateY(-50%);
  overflow: hidden;
} */
.slide {
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.slide-list {
  display: block;
  overflow: hidden;
  margin: auto;
  height: 90%;
  width: 100%;
  margin-top: 10px;
  list-style: none;
  position: relative;
}

.slide-img{
  width: 100%;
  height: 100%;
}
.slide-img input{
  display: none;
}

.slide-img label {
  width: 15px;
  height: 10px;
  border-radius: 50%;
  background-color: #000;
  display: flex;
  align-items: center;
  justify-content: center;
  /* position: absolute; */
}

.slide-img img{
  position: absolute;
  width: 50%;
  height: 100%;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  border-radius: 5px;
  align-items: center;
}
.slide-img img:nth-child(1) {
  left: 0;
  z-index: 1;
  transform: translateX(-100%) scale(.8);
}

.slide-img img:nth-child(2) {
  left: 0;
  z-index: 2;
  transform: translateX(-50%) scale(.8);
}

.slide-img img:nth-child(3) {
  left: 50%;
  z-index: 4;
  transform: translateX(-50%) scale(1);
}

.slide-img img:nth-child(4) {
  left: 100%;
  z-index: 2;
  transform: translateX(-50%) scale(.8);
}



.slide-prev img,
.slide-next img{
  position: absolute;
  top: 50%;
  z-index: 4;
  width: 100%;
  height: 30%;
  transform: translateX(-50%) translateY(-50%) scale(.8);
  cursor: pointer;
}

.slide-prev img {
  left: 200px;
}

.slide-next img {
  left: 1300px;
}

.slide-list:before,
.slide-list:after {
  display: block;
  /* content: ""; */
  position: absolute;
  /* top: 0; */
  width: 20%;
  height: 100%;
  z-index: 3;
}
/* .slide-list:before {
  left: 0;
  background-image:  linear-gradient(to right, rgba(0,0,0,1) 0%, rgba(0,0,0,0) 100%);
}

.slide-list:after {
  right: 0;
  background:  linear-gradient(to left, rgba(0,0,0,1) 0%, rgba(0,0,0,0) 100%);
} */
</style>