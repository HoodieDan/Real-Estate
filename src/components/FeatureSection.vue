<template>
  <div id="Services" class="bg">
    <div class="container">
        <div class="row">
            <div class="col-lg-4 col-md-4 text-center feature">
                <h4 class="feat mb-3">Buy A Home</h4>
                <p>We have saved a lot of customers millions.
                    Let us help you find your dream home at an
                    affordable rate with the best payment plan.</p>
                <button class="btn mt-4">Get Started<i class="fa-solid fa-chevron-right mx-3"></i></button>
            </div>
            <div class="col-lg-4 col-md-4 text-center feature">
                <h4 class="feat mb-3">Rent A Home</h4>
                <p>Are you looking to rent a space or apartment for a period of time? 
                    We got you covered.</p>
                <button class="btn mt-4">Get Started<i class="fa-solid fa-chevron-right mx-3"></i></button>
            </div>
            <div class="col-lg-4 col-md-4 text-center feature">
                <h4 class="feat mb-3">Sell A Home</h4>
                <p>What's your home worth? 
                    With our outlet, you can sell your home at the appropriate face value it was purchased or built.</p>
                <button class="btn mt-4">Get Started<i class="fa-solid fa-chevron-right mx-3"></i></button>
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
.bg {
    background-color: #494949;
    color: #fff;
    padding: 3.5rem 1rem;
}
.feature {
    padding: 1rem 2.5rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}
.feat {
    font-weight: 600;
    font-size: 1.7rem;
}
.feature p {
    font-size: 0.9rem;
    font-weight: lighter;
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
</style>