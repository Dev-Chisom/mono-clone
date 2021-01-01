<template>
  <main class="mono-landing__hero">
    <div class="container">
      <div class="mono-landing__left">
        <h1 class="mono-landing__heading">
          Access financial <br />
          accounts across <span>Africa with mono</span>
        </h1>
        <p class="text show-lg">
          Mono helps digital businesses in Africa access their customers'
          financial and identity data
        </p>
        <!-- <p class="text show-sm">
          Mono helps digital businesses in Africa access their customers' data
        </p> -->
        <div class="buttons">
          <a href="" class="mono-btn mono-btn-lg white mb-2 mr-1"
            >Start now <i class="fas fa-arrow-right"></i
          ></a>
          <a href="" class="mono-btn mono-btn-lg crystal mb-2"
            >Talk to an expert <i class="fas fa-headset"></i
          ></a>
        </div>
      </div>
      <div class="mono-landing__hero__right show-lg">
        <div class="mono-landing__hero__img img-1">
          <img src="../assets/images/landing-hero-laptop.png" alt="laptop" />
        </div>
        <div class="mono-landing__hero__img float img-2">
          <img src="../assets/images/landing-hero-phone.svg" alt="phone" />
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'hero',
};
</script>

<style scoped>
.mono-landing__hero {
  color: #fff;
  width: 100%;
  margin-top: 4rem;
}
.mono-landing__hero .container {
  /* display: flex;
  align-items: stretch;
  justify-content: space-between;
  flex-wrap: wrap;
  position: relative;
  z-index: 1000;
  margin-top: 2rem; */
  display: grid;
  gap: 5rem;
  grid-template-columns: 2fr 1fr;
  position: relative;
  z-index: 1000;
  margin-top: 5rem;
}
.mono-landing__left {
  position: relative;
  margin-right: 2rem;
  /* flex: 1.4; */
}
.mono-landing__heading {
  margin-bottom: 3.5rem;
  font-size: 4rem;
  max-width: 55rem;
  line-height: 1.1;
}
.mono-landing__heading h1 {
  /* font-size: 4.63vw; */
  /* line-height: 0.5; */
  font-weight: 700;
}

.mono-landing__heading span {
  display: block;
}
.mono-landing__left .text {
  margin-bottom: 5rem;
  font-size: 1.5rem;
  line-height: 1.5;
}
.mono-landing__left .buttons {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
.white {
  color: #182cd1;
  background: hsla(0, 0%, 100%, 0.9);
}
.white i {
  color: #182cd1;
}
.mono-landing__hero__right {
  /* flex: 1; */
  position: relative;
  min-width: 25rem;
}
.mono-landing__hero__img {
  animation: float 10s ease-in-out infinite;
  animation-delay: 3s;
  position: relative;
  margin-right: -10rem !important;
  height: auto;
  /* margin-right: auto; */
}
.mono-landing__hero__img .img-1 {
  width: 200% !important;
  /* margin-right: -20rem !important; */
}
.mono-landing__hero__img .img-2 {
  width: 100%;
}
.float {
  position: absolute;
  left: -10%;
  top: 30%;
  width: 15vw;
  max-width: 23rem;
  animation: float 8s ease-in-out infinite;
  /* margin-right: auto; */
}
@keyframes float {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-3%);
  }
  100% {
    transform: translateY(0);
  }
}
</style>
