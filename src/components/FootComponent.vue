<template>
    <div id="footer">
        <div class="container-fluid">
            <section class="row text-center justify-content-center p-3">
                <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex flex-column px-5 gap-3">
                    <div class="col-12 text-start">
                        <span class="fw-bolder t_size">CALL OUR EXPERTS TODAY 1.800.555.6789</span>
                    </div>

                    <div class="col-12 d-flex">
                        <div class="col-10 text-start t_two">
                            <span>©Copyright2012-2020 | Avada Theme by Theme Fusion | All Right Reserved | Powered by WordPress</span>
                        </div>

                        <div class="col-sm-1 col-lg-2 text-end">
                            <a href="#">c</a>
                            <a href="#">c</a>
                            <a href="#">c</a>
                            <a href="#">c</a>
                        </div>

                    </div>
                </div>
            </section>

            <div class="btn_c p-0">
                <div class="arrow p-2">
                    <font-awesome-icon icon="fa-solid fa-angle-up" />
                </div>
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

        .arrow{
            position: relative;
            transition: all .35s;
            width: 100%;
            height: 100%;

            &:after{
                position: absolute;
                content: "";
                top: 0;
                left: 0;
                width: 0;
                width: 100%;
                background: $col-four;
                border-radius: 5px 5px 0px 0px;
                transition: all 1s;
            } 

            &:hover{
                color: $col-two;
            }

            &:hover:after{
                height: 100%;
            }

            .fa-angle-up{
                position: relative;
                z-index: 2;
            }

        }
    }
}
</style>