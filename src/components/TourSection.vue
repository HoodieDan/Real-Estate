<template>
  <div id="Tour">
    <div class="bg-grey">
        <div class="container">
            <div class="row">
                <div class="col-lg-8 col-md-8 col-sm-8">
                    <h4 class="head mb-3">Tour Our Apartments</h4>
                    <p>All our apartments are equipped with accessories that make a house a home that meets all your luxury standards.</p>
                </div>
                <div class="col-lg-4 col-md-4 col-sm-4">
                    <button class="btn mt-4">View More<i class="fa-solid fa-chevron-right mx-3"></i></button>
                </div>
            </div>
        </div>
    </div>
    <div class="normal">
        <div class="container">
            <Slider />
        </div>
    </div>
  </div>
</template>

<script>
import Slider from './Slider.vue';
export default {
    components: { Slider }
}
</script>

<style scoped>
#Tour {
    /* height: 100vh; */
    position: relative;
}
.bg-grey {
    padding-top: 3rem;
    background-color: #494949;
    color: #FFF;
    height: 20rem;
}
.head {
    font-weight: 600;
    font-size: 1.7rem;
}
p {
    font-size: 0.9rem;
    width: 90%;
}
.col-lg-4 {
    text-align: right;
}
button.btn {
  background-color: #D9D849;
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
div.normal {
    position: relative;
    bottom: 8rem;
}
@media (max-height: 768px) {
    .bg-grey {
        height: 17rem;
    }
    div.normal {
        bottom: 4rem;
    }
}
@media (max-width: 575px) {
    .col-lg-4 {
        text-align: left;
    }
    .bg-grey {
        height: 30rem;
    }
    div.normal {
        bottom: 10rem;
    }
}
@media (max-width: 279px) {
    div.normal {
        bottom: 6rem;
    }
}
</style>