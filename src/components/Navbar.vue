<template>
  <div>
    <nav>
      <div class="mono-landing__container">
        <div class="mono-landing__logo">
          <img src="../assets/images/white.svg" alt="mono" />
        </div>
        <div class="mono-landing__nav">
          <ul class="mono-landing__nav--links">
            <li><a href="#" class="mono-landing__nav--items">Products</a></li>
            <li><a href="#" class="mono-landing__nav--items">Use Cases</a></li>
            <li><a href="#" class="mono-landing__nav--items">Pricing</a></li>
            <li><a href="#" class="mono-landing__nav--items">Docs</a></li>
            <li><a href="#" class="mono-landing__nav--items">Company</a></li>
          </ul>
        </div>
        <div class="mono-landing__lists">
          <img src="../assets/images/nigeria.svg" alt="Nigeria" />
          <a href="#" class="mono-btn crystal"
            >Login <i class="fas fa-arrow-right"></i
          ></a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'navbar',
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
  font-size: 1rem;
  color: #fff;
  padding: 0.7rem;
  font-weight: 500;
  border-radius: 0.7rem;
  font-size: 1.5rem;
  transition: all 0.3s cubic-bezier(0.785, 0.135, 0.15, 0.86);
}
</style>
