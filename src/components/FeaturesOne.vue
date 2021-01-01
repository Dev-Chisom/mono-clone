<template>
  <main>
    <section class="mono-landing__clients">
      <div class="container">
        <h5 class="mono-landing__clients--heading">
          Trusted by businesses like
        </h5>
        <div class="mono-landing__clients--logos">
          <div class="mono-landing__clients--logo">
            <img src="../assets/images/carbon.svg" alt="carbon" />
          </div>
          <div class="mono-landing__clients--logo">
            <img src="../assets/images/zedvance.png" alt="carbon" />
          </div>
          <div class="mono-landing__clients--logo">
            <img src="../assets/images/indicima.png" alt="carbon" />
          </div>
          <div class="mono-landing__clients--logo">
            <img src="../assets/images/flutterwave.svg" alt="carbon" />
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: 'FeaturesOne',
};
</script>

<style scoped>
.mono-landing__clients {
  padding: 5rem 13rem 3rem;
  position: relative;
}
.mono-landing__clients .container {
  padding: 0 10rem;
  position: relative;
}
.mono-landing__clients .container::before {
  position: absolute;
  content: '';
  right: 95%;
  height: 25px;
  width: 100%;
  background-image: linear-gradient(
    90deg,
    #e4edfb 50%,
    rgba(237, 243, 252, 0) 0
  );
  background-position: 50%;
  background-size: 12px 1px;
  background-repeat: repeat-x;
}
.mono-landing__clients--heading {
  font-weight: 400;
  margin-bottom: 4rem;
  color: #55586f;
  font-size: 1.4rem;
}
.mono-landing__clients--logos {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  align-items: center;
  gap: 5rem;
  padding-bottom: 2rem;
  /* display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative; */
}
.mono-landing__clients--logo {
  display: flex;
  align-items: center;
  max-width: 16rem;
  min-width: 8rem;
  cursor: pointer;
  position: relative;
}
.mono-landing__clients--logos::after {
  position: absolute;
  content: '';
  left: 0;
  height: 3rem;
  width: 200%;
  top: 100%;
  background-image: linear-gradient(
    90deg,
    #e4edfb 50%,
    rgba(237, 243, 252, 0) 0
  );
  background-position: bottom;
  background-size: 12px 1px;
  background-repeat: repeat-x;
}
</style>
