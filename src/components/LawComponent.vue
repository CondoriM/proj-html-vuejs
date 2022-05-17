<template>
    <div class="container-fluid">
        <section id="law" class="row text-center justify-content-center p-5 bg_second">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex justify-content-center">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="row border_t">
                    <div class="col-4  p-4 bg_first" v-for="(col,index) in law" :key="col + index">
                        <img :src="require(`../assets/img/${col.img}`)" alt="">
                        <h5 class="p-3">{{col.title}}</h5>
                        <p class="mb-5 t_one">{{col.text}}</p>
                    </div>
                </div>
            </div>

            <div class="row my_row text-center justify-content-center">
                <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex gap-xl-3 justify-content-around align-items-center">

                    <!-- sezione logo -->
                    <div class="col-xl-3 col-2">
                        <img src="@/assets/img/avada-law-logo.png" alt="">
                    </div>

                    <!--  -->
                    <div class="col-8 col-xxl-10 bar">
                        <span class="d-flex justify-content-between bar">
                            <a class="d-flex align-items-center bar" href="#"><span>Home</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>Who We Are</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>What We Do</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>Where We Work</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>Careers</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>News</span></a>
                            <a class="d-flex align-items-center bar" href="#"><span>Contact</span></a>
                        </span>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    data(){
        return{
            law:[
                {img: 'law_7.jpg', title: 'INTERNATIONAL',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'},
                {img: 'law_8.jpg', title: 'PARTNERSHIPS',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'},
                {img: 'law_3.jpg', title: 'EXCELLENCE',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'}
            ],
        }
    }
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
</style>
