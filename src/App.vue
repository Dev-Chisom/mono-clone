<template>
  <div id="app">
    <header>
      <Navbar />
      <Hero />
    </header>
    <FeaturesOne />
  </div>
</template>

<script>
import Navbar from './components/Navbar';
import Hero from './components/Hero';
import FeaturesOne from './components/FeaturesOne';
export default {
  name: 'app',
  components: {
    Navbar,
    Hero,
    FeaturesOne,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'DM Sans', sans-serif;
  overflow-x: hidden;
}
header {
  width: 100vw;
  background: url('./assets/images/hero-blue.svg');
  background-position: 0 100%;
  background-repeat: no-repeat;
  background-size: cover;
  margin-bottom: 5rem;
  position: relative;
}
a {
  text-decoration: none;
  transition: all 0.3 ease-in;
  font-weight: 400;
}
ul {
  list-style: none;
}
.crystal {
  background: hsla(0, 0%, 100%, 0.1);
  backdrop-filter: blur(15px);
}
img {
  width: 100%;
}
.white {
  color: #182cd1;
  background: hsla(0, 0%, 100%, 0.1);
}
.mb-1 {
  margin-bottom: 1rem !important;
}
.mb-2 {
  margin-bottom: 4.5rem !important;
}
.mr-1 {
  margin-right: 1rem !important;
}
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}
i {
  font-size: 1rem;
  color: #fff;
}
.mono-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  font-size: 1rem;
  color: #fff;
  padding: 0.5rem;
  font-weight: 500;
  border-radius: 0.7rem;
  font-size: 1rem;
  transition: all 0.3s cubic-bezier(0.785, 0.135, 0.15, 0.86);
  box-shadow: 0 3px 5px rgba(0, 0, 0, 0.1);
}
.mono-btn-lg {
  padding: 1rem 2rem;
}
</style>
