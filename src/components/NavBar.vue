<template>
  <nav class="fixed-top">
    <div class="container">
        <div>
            <div>
                <a class="navbar-brand logo green" href="#">
                Real<span class="yellow">Estate</span>
                </a>
            </div>
        </div>
        <div class="navi-items">
            <button class="navbar-toggle" type="button" aria-label="Toggle navigation" 
            :class="{ 'aside-color': navIsOpen }"
            @click="toggleNav">
                <span class="toggler-icon top-bar"
                :class="{ 'top-icon-animate': navIsOpen }"></span>
                <span class="toggler-icon middle-bar"
                :class="{ 'middle-icon-animate': navIsOpen }"></span>
                <span class="toggler-icon bottom-bar"
                :class="{ 'bottom-icon-animate': navIsOpen }"></span>
            </button>
            <ul class= "navbar-navi">
                <li class="navbar-item">
                <a class="navbar-link" href="#Home">Home</a>
                </li>
                <li class="navbar-item">
                <a class="navbar-link" href="#Service">Service</a>
                </li>
                <li class="navbar-item">
                <a class="navbar-link" href="#About">About</a>
                </li>
                <li class="navbar-item">
                <a class="navbar-link" href="#Contact">Contact</a>
                </li>
                <li class="navbar-item">
                    <button class="btn">Sign in</button>
                </li>
            </ul>
        </div>
    </div>
  </nav>

  <!-- Mobile Navigation -->
  <div
    class="backdrop"
    @wheel.prevent
    @touchmove.prevent
    @scroll.prevent
    @touch.self="toggleNav"
    @click.self="toggleNav"
    :class="{ 'open': navIsOpen }"
  >
    <aside>
      <a class="navbar-link mono block light-slate" href="#Home" @click="toggleNav">Home</a>
      <a class="navbar-link mono block light-slate" href="#Services" @click="toggleNav">Services</a>
      <a class="navbar-link mono block light-slate" href="#About" @click="toggleNav">About</a>
      <a class="navbar-link mono block light-slate" href="#Contact" @click="toggleNav">Contact</a>
      <a class="navbar-link mono block light-slate" href="#" @click="toggleNav">
      <button class="btn">Sign in</button>
      </a>
    </aside>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      navIsOpen: false,
    }
  },
  methods: {
    toggleNav() {
      this.navIsOpen = !this.navIsOpen;
    }
  }
}
</script>

<style scoped>
nav {
  background-color: #F5F5F5;
  color: #494949;
  position: relative;
  height: 80px;
  width: 100%;
  padding: 2rem 1.5rem;
}
div.container {
  display: flex;
  justify-content: space-between;
}
li {
  font-size: 0.8rem;
}
button.navbar-toggle {
  background-color: #F5F5F5;
  border-style: none;
  display: none;
  position: relative;
  cursor: pointer;
  width: 30px;
  height: 30px;
  z-index: 1000;
}
span.top-bar {
  margin-top: -8px;
  transform: rotate(0deg);
  border-radius: 32px;
}
span.middle-bar {
  opacity: 1;
  filter: alpha(opacity=100);
  width: 85%;
  border-radius: 32px;
}
span.bottom-bar {
  margin-top: 8px;
  width: 70%;
  transform: rotate(0deg);
  border-radius: 32px;
}
/* ul.navbar-navi {
  position: relative;
  right: 30%;
} */
li.navbar-item {
  margin: 0 0 0 5rem;
}
a.navbar-link {
  transition: all 0.2s;
  color: #494949;
}
a.navbar-link:hover {
  color: #D9D849;
}
.toggler-icon {
  display: block;
  display: none;
  position: absolute;
  height: 3px;
  width: 100%;
  background: #494949;
  border-radius: 1px;
  opacity: 1;
  left: 0;
  transform: rotate(0deg);
  transition: .25s ease-in-out;
}
.navbar-brand {
    font-weight: 600;
}
.navi-items {
  display: flex;
}
.navbar-navi {
  display: flex;
  justify-content: space-around;
  font-weight: 500;
}
.top-icon-animate {
  margin-top: 0px !important;
  transform: rotate(135deg) !important;
}
.middle-icon-animate {
  opacity: 0 !important;
  filter: alpha(opacity=0) !important;
}
.bottom-icon-animate {
  margin-top: 0px !important;
  transform: rotate(-135deg) !important;
  width: 100% !important;
}
button.btn {
  background-color: #D9D849;
  border: #F5F5F5 1px solid;
  white-space: nowrap;
  text-align: center;
  color: #F5F5F5;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
  font-size: 0.9rem;
  position: relative;
  bottom: 0.5rem;
  transition: all 0.2s linear;
}
button.btn:hover {
  background-color: #a7a723;
}
div.backdrop {
    position: fixed;
    overflow: hidden;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    backdrop-filter: blur(5px);
    transform: scale(0, 0);
    transition: all 0.5s;
    z-index: 10;
}
aside {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  position: fixed;
  width: 100vw;
  height: 70vh;
  top: 0;
  background-color: #F5F5F5;
  color: #494949;
  text-align: center;
  /* transform: translateX(1000px); */
  z-index: 10;
  padding: 80px 10px;
  transition: all 0.5s;
}
.open {
  transform: scale(1, 1) !important;
}
@media (max-width: 930px) {
  li.navbar-item {
  margin: 0 0 0 3rem;
}
}
@media (min-width: 769px) {
    aside {
        display: none;
    }
}
/* @media (max-width: 820px) {
    nav {
        padding-top: 3%;
    }
} */
@media (max-width: 768px) {
  ul.navbar-navi {
    display: none;
  }
  button.navbar-toggle {
    display: block;
    margin-right: 10px;
    z-index: 11;
  }
  .toggler-icon {
    display: block;
  }
  div.container {
    padding: 0 !important;
  }
}
@media (max-height: 700px) {
  aside {
    padding: 80px 10px 25px;
  }
  aside a {
    padding-top: 20px;
  }
}
</style>