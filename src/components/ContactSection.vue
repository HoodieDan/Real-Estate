<template>
  <div id="Contact">
    <div class="container">
        <div class="row">
            <div class="col-lg-7 col-md-7">
                <img class="img-fluid" src="../assets/images/contact-section-img.png" alt="Contact us">
            </div>
            <div class="col-lg-4 col-md-4">
                <h4 class="head mb-5">The Leading Real Estate
                    Rental Marketplace</h4>
                <p class="mb-4">From vast lands to a conducive environment, we provide well structured and equipped apartments for your utmost comfort and security.</p>
                <p>At Real Estate, it’s not about selling homes. It’s about serving families. We have built a home that guarantees comfort, luxury and
                    style at an affordable rate for your family.</p>
                    <button class="btn mt-4">Contact Us<i class="fa-solid fa-chevron-right mx-3"></i></button>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
#Contact {
    height: 100vh;
    padding: 5rem;
    color: #494949;
    display: flex;
    align-items: center;
}
p {
    font-size: 0.9rem;
}
.row {
    align-items: center;
}
img {
    width: 80%;
}
.head {
    font-weight: 600;
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
@media (max-width: 768px) {
    #Contact {
        height: auto;
    }
    img {
        width: auto;
        margin-bottom: 2rem;
    }
}
@media (max-width: 440px) {
    #Contact {
        padding: 4rem 2rem;
    }
}
</style>