<template>
  <div class="container">
    <img class="moon" src="@/assets/home/moon.svg" alt="moon" />
    <div class="logo">
      <img src="@/assets/home/logo.svg" alt="" />
    </div>
    <Link />,
 

    <img class="cloud1" src="@/assets/cloud1.svg" alt="" />
  </div>
</template>

<script>
import Link from './Link.vue'
export default {
   components: {
    Link
  }
};
</script>


<style scoped>
.container {
  position: relative;
}
.moon{
  width: 60px;
  display: block;
  position: absolute;
  left: 15%;
  transform: rotate(-10deg);
  animation: moon 4s reverse;
}
/* logo */
.logo {
  margin-top: 100px;
}
.logo img {
  margin: 30px;
  margin: 0 auto;
  width: 240px;
  /* height: 15/0px; */
}
a,
img {
  display: block;
}


.cloud1 {
  width: 150px;
  position: absolute;
  right: 15%;
  bottom: 0;
  animation: clound 4s infinite
}

@keyframes clound {
  0%, 100% {
    transform: translateY(0px);
  }
  50%{
    transform: translateY(-15px);
    }
}
@keyframes moon {
  0% , 100%{
    transform: rotate(-20deg);
  }
  30%{
    transform: rotate(-20deg);
  }
  50%{
    transform: rotate(-50deg);
    }
  60%{
    transform: rotate(0deg);
    }
}

@media(max-width:1024px){
.moon{
  width: 42px;
  left: 15%;
  top: 0;
}
/* logo */
.logo {
  margin-top: 50px;
}
.logo img {
  margin: 3px auto;
  width: 200px;
}
.links ul {
  margin-top: 15px;
  gap: 15px;
}
ul li a img {
  width:42px;
  height: auto;
}

.cloud1 {
  width: 100px;
  right: 15%;
  bottom: 0;
}
}
@media(max-width:768px){
  .moon{
  width: 42px;
  left: 15%;
  top: 20%;
}
/* logo */
.logo {
  margin-top: 50px;
}
.logo img {
  margin: 3px auto;
  width: 220px;
}
.links ul {
  margin-top: 15px;
  gap: 15px;
}
ul li a img {
  width:47px;
  height: auto;
}

.cloud1 {
  width: 100px;
  right: 15%;
  bottom: 40%;
}
}
@media(max-width:615px){
  .moon{
  width: 40px;
  left: 10%;
  top: -4%;
}
/* logo */
.logo {
  margin-top: 50px;
}
.logo img {
  margin: 3px auto;
  width: 220px;
}
.links ul {
  margin-top: 15px;
  gap: 15px;
}
ul li a img {
  width:47px;
  height: auto;
}

.cloud1 {
  width: 90px;
  right: 4%;
  bottom: 17%;
}
}
@media(max-width:425px){
  .moon{
  width: 34px;
  left: 10%;
  top: -4%;
}
/* logo */
.logo {
  margin-top: 50px;
}
.logo img {
  margin: 3px auto;
  width: 220px;
}
.links ul {
  margin-top: 15px;
  gap: 15px;
}
ul li a img {
  width:47px;
  height: auto;
}

.cloud1 {
  width: 80px;
  right: 4%;
  bottom: 17%;
}
}
@media(max-width:375px){
  .moon{
  width: 30px;
  left: 8%;
  top: -3%;
}
/* logo */
.logo {
  margin-top: 50px;
}
.logo img {
  margin: 3px auto;
  width: 220px;
}
.links ul {
  margin-top: 15px;
  gap: 15px;
}
ul li a img {
  width:47px;
  height: auto;
}

.cloud1 {
  width: 65px;
  right: 4%;
  bottom: 20%;
}
}
</style>
