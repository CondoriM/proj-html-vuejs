<template>
    <div class="container-fluid">

        <!-- Prima sezione main -->
        <div id="first" class="row text-center justify-content-center p-5 bg_second">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex justify-content-center">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="row border_t">
                    <div class="col-4 p-4 bg_first" v-for="(col,index) in 3" :key="col + index">
                        <h5>WHO WE  ARE</h5>
                        <p class="mb-3 t_one">Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.</p>
                        <a class="btn_c grow" href="#"><span>LEARN MORE</span></a>
                    </div>
                </div>
            </div>
        </div>

        <!-- Seconda sezione main -->
        <section id="global" class="row text-center justify-content-center p-5">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex justify-content-around ">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="col-3 p-3" v-for="(col,index) in 4" :key="col + index">
                    <font-awesome-icon class="check" icon="fa-solid fa-check" />
                    <h5>A GLOBAL VIEW</h5>
                    <p class="t_one">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta illum, corporis vero a id facere!</p>
                </div>
            </div>
        </section>
        
        <!-- Section ask -->
        <section id="ask" class="row text-center justify-content-center p-5">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex justify-content-center">
                <div class="col-10 col-sm-8">
                    <h5 class="text-start">
                        QUESTION ABOUT A JUDICIAL ISSUE? ASK OUR EXPERTS.
                    </h5>
                </div>

                <!-- Button -->
                <div class="col-2 col-sm-3 d-flex align-items-center">
                    <a class="btn_c t_size fw-bolder" href="#">
                        <span>ASK AN EXPERT</span>
                    </a>
                </div>
            </div>
        </section>

        <ChallengeComp/>

        <!-- sezione envato -->
        <section id="envato" class="row text-center justify-content-center p-5 bg_third">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 flex-column">
                <img class="mb-3" src="@/assets/img/envato-logo.png" alt=""><br>
                <span class="fst-italic">"We have worked with Avada Law for the past 15 years. As we have grown and evolved, what i have value most about our relationship is that Avada Law knowus and our business"</span>
                <p class="p-3 fw-bolder t_size">Nigel Rawlinson • Senior Partner</p>
            </div>
        </section>

        <!-- Sezione Law -->
        <LawList/>

        <section id="together" class="row text-center justify-content-center p-5 ">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex flex-column align-items-center">
                <h4>LET'S WORK TOGETHER</h4>

                <!-- linea decorativa -->
                <div class="col-2 p-4">
                    <hr>
                </div>

                <div class="col-9 ">
                    <p class="fw-bolder mb-4">We work as a single united team with market leading firms around the world and give our clients the highest quality advice possible.</p>

                    <a class="btn_c my-5 fw-bold" href="#"><span>MAKE ENQUIRY</span></a>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
import LawList from '@/components/LawComponent.vue'
import ChallengeComp from '@/components/ChallengeComponent.vue'

export default {
    components:{
        LawList,
        ChallengeComp
    }, 
}
</script>


<style lang="scss" scoped>
@import '@/assets/scss/style.scss';
</style>