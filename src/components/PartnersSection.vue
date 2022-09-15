<template>
  <section id="Partners" class="mb-5">
    <div class="container text-center">
        <div class="our-partners mb-5">
            <h4>Our Partners</h4>
        </div>
        <div class="row mb-3">
            <div class="col-lg-3 col-md-3 col-sm-3 col-6 mb-5">
                <img src="../assets/images/access.png" alt="access bank" class="img-fluid">
            </div>
            <div class="col-lg-3 col-md-3 col-sm-3 col-6 mb-5">
                <img src="../assets/images/seedbuilders.png" alt="seed builders" class="img-fluid">
            </div>
            <div class="col-lg-3 col-md-3 col-sm-3 col-6 mb-5">
                <img src="../assets/images/julius-berger.png" alt="julius berger" class="img-fluid">
            </div>
            <div class="col-lg-3 col-md-3 col-sm-3 col-6 mb-5">
                <img src="../assets/images/interswitch.png" alt="interswitch" class="img-fluid">
            </div>
            <div class="col-lg-1 col-0"></div>
            <div class="col-lg-3 col-md-4 col-sm-4 col-6 mb-5">
                <img src="../assets/images/flutterwave.png" alt="flutterwave" class="img-fluid">
            </div>
            <div class="col-lg-4 col-md-4 col-sm-4 col-6 mb-5">
                <img src="../assets/images/e-health.png" alt="e-health" class="img-fluid">
            </div>
            <div class="col-lg-3 col-md-4 col-sm-4 mb-5">
                <img src="../assets/images/andela.png" alt="andela" class="img-fluid">
            </div>
            <div class="col-lg-1 col-0"></div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'PartnersSection'
}
</script>

<style scoped>
#Partners {
    padding: 4rem;
}
div.our-partners {
    display: inline-block;
    color: #FFFFFF;
    background-color: #D9D849;
    padding: 0.8rem 4.5rem;
}
.our-partners h4 {
    font-weight: 600;
    margin: 0;
    padding: 0;
}
@media (max-width: 400px) {
    #Partners {
        margin: 0 !important;
        padding: 3rem 1rem;
    }
}
</style>