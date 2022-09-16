<template>
  <div id="Home" class="container">
    <div class="hero">
        <div class="col-lg-7 col-md-9">
            <h1 class="heading">Turn A House To Your Home</h1>
            <p class="heading-baby mt-3">With over 1 million+ homes available,  we can match you with 
                a house you will want to call home.</p>
            <button class="btn mt-4">Explore<i class="fa-solid fa-chevron-right mx-3"></i></button>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'HeroSection',
}
</script>

<style scoped>
div.hero {
    color: #494949;
    height: 100vh;
    background-image: url('../assets/images/house.png');
    background-repeat: no-repeat;
    background-size: contain;
    background-position: bottom right;
}
h1.heading {
    font-weight: 700;
    font-size: 4.5rem;
    margin-top: 3rem;
}
.heading-baby {
    width: 80%;
    font-size: 0.9rem;
}
button.btn {
  background-color: #D9D849;
  border: #F5F5F5 1px solid;
  white-space: nowrap;
  text-align: center;
  color: #F5F5F5;
  padding-left: 2rem;
  padding-right: 1rem;
  font-size: 0.9rem;
  position: relative;
  bottom: 0.5rem;
  transition: all 0.2s linear;
}
button.btn:hover {
  background-color: #a7a723;
}
@media (max-width: 992px) {
  .hero {
    height: 60vh !important;
  }
}
@media (max-width: 575px) {
  .hero {
    height: 80vh !important;
  }
  .col-lg-7 {
    padding: 1rem;
  }
  h1.heading {
    font-size: 3.5rem;
  }
}
@media (max-width: 375px) {
  h1.heading {
    font-size: 2.5rem;
  }
  .col-lg-7 {
    padding: 0 0.5rem;
  }
}
@media (max-height: 500px) {
  h1.heading {
    margin-top: 1rem;
    font-size: 2rem;
  }
  .heading-baby {
    width: 90%;
    font-size: 0.8rem;
}
}
</style>