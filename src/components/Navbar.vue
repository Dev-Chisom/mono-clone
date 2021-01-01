<template>
  <div>
    <nav>
      <div class="mono-landing__container">
        <div class="mono-landing__logo">
          <img src="../assets/images/white.svg" alt="mono" />
        </div>
        <div class="mono-landing__nav">
          <ul class="mono-landing__nav--links">
            <li v-for="list in lists" :key="list">
              <a href="#" class="mono-landing__nav--items">{{ list }}</a>
            </li>
          </ul>
        </div>
        <div class="mono-landing__lists">
          <img src="../assets/images/nigeria.svg" alt="Nigeria" />
          <a href="#" class="mono-btn crystal"
            >Login <i class="fas fa-arrow-right"></i
          ></a>
        </div>
        <div @click="openMobileNav()" id="burger">
          <div class="line1"></div>
          <div class="line2"></div>
          <div class="line3"></div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'navbar',
  data() {
    return {
      lists: ['Products', 'Use Cases', 'Pricing', 'Docs', 'Company'],
    };
  },
  methods: {
    openMobileNav() {
      const burger = document.getElementById('burger');
      const nav = document.querySelector('.nav-links');
      const navLinks = document.querySelectorAll('.nav-links li');
      // Toggle navigation on mobile
      nav.classList.toggle('nav-active');
      // Burger toggler
      burger.classList.toggle('toggle');
      // Animate navigation links
      navLinks.forEach((link, index) => {
        if (link.style.animation || link.style.webkitAnimation) {
          link.style.animation = '';
          link.style.webkitAnimation = '';
        } else {
          link.style.webkitAnimation = `navLinkFade 0.5s ease forwards ${index /
            7}s`;
          link.style.animation = `navLinkFade 0.5s ease forwards ${index / 7}s`;
        }
      });
    },
  },
};
</script>

<style scoped>
nav {
  max-width: 1200px;
}
.mono-landing__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: relative;
  padding-top: 2.3rem;
}
.mono-landing__logo {
  height: 1.665rem;
  /* margin-right: 5rem; */
  margin-left: 3rem;
  display: inline-block;
}
.mono-landing__logo img {
  height: 100%;
  width: inherit;
}
.mono-landing__nav--links {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.mono-landing__nav--items {
  padding: 1.2rem;
  color: #fff;
}
.mono-landing__lists {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.mono-landing__lists .mono-btn {
  padding-left: 1rem;
  margin-left: 1.5rem;
}
.crystal {
  background: hsla(0, 0, 100%, 0.1);
  backdrop-filter: blur(15px);
}
.mono-landing__lists i {
  font-size: 1rem;
  color: #fff;
}
.mono-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  font-size: 1rem !important;
  color: #fff;
  padding: 0.7rem;
  font-weight: 500;
  border-radius: 0.7rem;
  font-size: 1.5rem;
  transition: all 0.3s cubic-bezier(0.785, 0.135, 0.15, 0.86);
}
#burger {
  display: none;
  cursor: pointer;
}
#burger div {
  width: 30px;
  height: 3px;
  margin: 8px;
  background-color: #fefefe;
  transition: all 0.3s ease-in;
}

@media screen and (max-width: 768px) {
  #burger {
    display: block;
  }
}
.nav-active {
  transform: translateX(0) !important;
}
@keyframes navLinkFade {
  from {
    opacity: 0;
    transform: translateX(-60px);
  }
  to {
    opacity: 1;
    transform: translateX(0px);
  }
}
.toggle .line1 {
  transform: rotate(-45deg) translate(-9px, 10px);
}
.toggle .line2 {
  opacity: 0;
}
.toggle .line3 {
  transform: rotate(45deg) translate(-5px, -6px);
}
</style>
