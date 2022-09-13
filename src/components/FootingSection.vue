<template>
  <footer id="About">
    <div class="container">
        <div class="row">
            <div class="col-lg-6">
                <h5 class="mb-4">Real Estate</h5>
                <p>Real Estate is the leading estate rental marketplace. 
                    With over 1 million+ homes available, we can match 
                    you with a house you will want to call home.</p>
                <p><i class="fa-solid fa-location-dot"></i> Brooklyn, New York, United States</p>
                <p><i class="fa-solid fa-phone"></i> +123 456 789</p>
                <p><i class="fa-solid fa-envelope"></i> help@realestate.com</p>
            </div>
            <div class="col-lg-2 col-4">
                <h6 class="mb-4">Company</h6>
                <a href="#">About Us</a>
                <a href="#">Blog</a>
                <a href="#">All Products</a>
            </div>
            <div class="col-lg-2 col-4">
                <h6 class="mb-4">Services</h6>
                <a href="#">Buy A Home</a>
                <a href="#">Sell A Home</a>
                <a href="#">Rent A Home</a>
            </div>
            <div class="col-lg-2 col-4">
                <h6 class="mb-4">Customer Care</h6>
                <a href="#">Login</a>
                <a href="#">Sign Up</a>
                <a href="#">FAQ</a>
                <a href="#">Contact Us</a>
            </div>
        </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
footer {
    background-color: #D9D9D9;
    color: #494949;
    padding: 4rem;
}
h5,h6 {
    font-weight: 600;
}
p {
    font-size: 0.9rem;
    width: 90%;
}
a {
    display: block;
    font-size: 0.9rem;
    margin: 1rem 0;
    color: #494949;
    transition: all 0.3s;
}
a:hover {
    color: #D9D849;
}
@media (max-width: 992px) {
    .col-lg-6 {
        margin-bottom: 2rem;
    }
}
@media (max-width: 575px) {
    footer {
        padding: 4rem 1rem;
    }
}
</style>