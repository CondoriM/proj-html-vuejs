<template>
    <div id="footer">
        <div class="container-fluid">
            <section class="row text-center justify-content-center p-3">
                <div class="col-10 d-flex flex-column px-5">
                    <div class="col-12 text-start">
                        <span>CALL OUR EXPERTS TODAY 1.800.555.6789</span>
                    </div>

                    <div class="col-12 d-flex">
                        <div class="col-10 text-start">
                            <span>©Copyright2012-2020 | Avada Theme by Theme Fusion | All Right Reserved | Powered by WordPress</span>
                        </div>

                        <div class="col-2 text-end">
                            <a href="#">c</a>
                            <a href="#">c</a>
                            <a href="#">c</a>
                            <a href="#">c</a>
                        </div>

                    </div>
                </div>
            </section>

            <div class="btn_c px-3">
                <font-awesome-icon icon="fa-solid fa-angle-up" />
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/style.scss';

#footer{
    position: relative;

    .btn_c{
        position: absolute;
        bottom: 0;
        background-color: $med-two;
        right: 3rem;
        border-radius: 5px 5px 0px 0px;
    }
}
</style>