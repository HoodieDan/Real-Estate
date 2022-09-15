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
    height: 100vh;
    position: relative;
}
.bg-grey {
    padding-top: 3rem;
    background-color: #494949;
    color: #FFF;
    height: 50%;
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
    bottom: 20%;
}
@media (max-width: 992px) {
    div.normal {
        bottom: 15%;
    }
}
@media (max-width: 820px) {
  #Tour {
    height: 60vh !important;
  }
}
@media (max-width: 575px) {
    #Tour {
        height: 100vh !important;
    }
    .col-lg-4 {
        text-align: left;
    }
}
@media (max-width: 440px) {
    .bg-grey {
        padding: 3rem 1rem;
        height: 50vh;
    }
    div.normal {
        height: auto;
        bottom: 10%;
    }
    /* #Tour {
        height: 80vh;
    } */
}
@media (max-width: 350px) {
    #Tour {
        height: auto;
    }
    .bg-grey {
        height: 60vh;
    }
    div.normal {
        height: auto;
        bottom: 5%;
    }
}
</style>