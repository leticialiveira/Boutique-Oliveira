<script  >
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
  <div class="slide-list">
    <div class="slide-prev"><img src="../assets/icons/arrow-left.svg" alt=""></div>
    <div class="slide-next"><img src="../assets/icons/arrow-right.svg" alt=""></div>
    <div class="slide">
        <img class="slide-img" src="../assets/image/teste.jfif" alt="">
        <img class="slide-img" src="../assets/image/teste2.jfif" alt="">
        <img class="slide-img" src="../assets/image/teste3.jfif" alt="">
        <img class="slide-img" src="../assets/image/teste4.jfif" alt="">
    </div>
</div>
</template>

<style>
.slide {
  position: relative;
  top: 50%;
  transform: translateY(-50%);
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  /* overflow: hidden; */
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

.slide-img {
  position: absolute;
  width: 50%;
  height: 100%;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
  border-radius: 5px;
  align-items: center;
}
.slide-img :nth-child(1) {
  left: 0;
  z-index: 1;
  transform: translateX(-100%) scale(.8);
}

.slide-img :nth-child(2) {
  left: 0;
  z-index: 2;
  transform: translateX(-50%) scale(.8);
}

.slide-img :nth-child(3) {
  left: 50%;
  z-index: 4;
  transform: translateX(-50%) scale(1);
}

.slide-img :nth-child(4) {
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