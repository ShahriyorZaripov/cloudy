<template>
  <div class="container">
    <div class="text">
      <div class="cnf_img">
        <img class="text_img_1" src="@/assets/about/cnf.svg" alt="" />
      </div>
      <div class="text_list_img">
        <img src="@/assets/about/cnf1.svg" alt="" />
        <img src="@/assets/about/cnf2.svg" alt="" />
      </div>
    </div>

    <div class="roadmap">
      <img class="roadmap_list_img" src="@/assets/about/roadmap.png" alt="" />
      <img
        class="roadmap_list_responsive"
        src="@/assets/about/roadmap2.png"
        alt=""
      />
    </div>
    <img class="cloud2" src="@/assets/cloud2.svg" alt="" />
    <img class="fr" src="@/assets/about/fr.png" alt="" />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.container {
  position: relative;
  padding: 0 60px;
  max-width: 1130px;
  margin: 150px auto 0;
  display: flex;
}
.text {
  flex: 1 1 10rem;
}

.text img {
  max-width: 130px;
  margin-bottom: 20px;
}
.text_img_1 {
  max-width: 140px !important;
}
.roadmap {
  /* border: 1px solid; */
  flex: 3 1 30rem;
}
.roadmap_img {
  width: fit-content;
  margin: 0 auto 40px;
  transform: translateX(90px);
}
.roadmap_list_img {
  width: 100%;
}
.roadmap_list_responsive {
  display: none;
}

.cloud2 {
  width: 150px;
  display: block;
  position: absolute;
  left: 5%;
  bottom: -4%;
  animation: clound 4s infinite;
}

.fr {
  width: 40px;
  display: block;
  position: absolute;
  transform: rotate(20deg);
  left: auto;
  right: 5%;
  bottom: -4%;
}

/* keyfrem */
@keyframes clound {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-15px);
  }
}
/* Responsive */
@media (max-width: 959px) {
  .roadmap {
    margin-top: 184px;
  }
  .cloud2 {
    width: 140px;
    top: 10%;
    right: 5%;
    left: auto;
    bottom: auto;
  }

  .fr {
    width: 35px;
    left: 12%;
    right: auto;
    bottom: 20%;
  }
}
@media (max-width: 768px) {
  .container {
    flex-direction: column;
    align-items: center;
    padding: 0 20px;
    margin: 50px auto 0;
  }
  .text {
    width: 320px;
  }
  .cnf_img {
    width: fit-content;
    margin: 0 auto;
  }
  .text_list_img {
    margin-bottom: 20px;
    display: flex;
    justify-content: space-around;
  }
  .roadmap {
    margin-top: 0;
  }
}
@media (max-width: 600px) {
  .roadmap_list_img {
    display: none;
  }
  .roadmap_list_responsive {
    width: 100%;
    display: block;
  }
  .cloud2 {
    width: 90px;
    top: 20%;
    right: 4%;
    left: auto;
    bottom: auto;
  }

  .fr {
    width: 30px;
    left: auto;
    right: 4%;
    bottom: 0;
  }
}
@media (max-width: 375px) {
  .text img {
    max-width: 110px;
    margin-bottom: 20px;
    padding: 0 10px;
  }
  .text_img_1 {
    max-width: 120px !important;
  }
  .cloud2 {
    width: 120px;
    top: auto;
    right: 5%;
    left: auto;
    bottom: 0;
  }

  .fr {
    width: 35px;
    left: 12%;
    right: auto;
    bottom: 0;
  }
}
</style>