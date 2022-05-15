<template>
    <div class="container-fluid">

        <!-- Prima sezione main -->
        <div class="row text-center justify-content-center p-5 bg_second">
            <div class="col-10 d-flex justify-content-center">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="row border_t">
                    <div class="col-4 p-4 bg_first" v-for="(col,index) in 3" :key="col + index">
                        <h5>WHO WE  ARE</h5>
                        <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.</p>
                        <a class="btn_c" href="#">LEARN MORE</a>
                    </div>
                </div>
            </div>
        </div>

        <!-- Seconda sezione main -->
        <section class="row text-center justify-content-center p-5">
            <div class="col-10 d-flex justify-content-around ">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="col-3 p-3" v-for="(col,index) in 4" :key="col + index">
                    <h5>A GLOBAL VIEW</h5>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta illum, corporis vero a id facere!</p>
                </div>
            </div>
        </section>
        
        <!-- Section ask -->
        <section id="ask" class="row text-center justify-content-center p-5 bg_third">
            <div class="col-10 d-flex">
                <div class="col-10">
                    <h5>
                        QUESTION ABOUT A JUDICIAL ISSUE? ASK OUR EXPERTS.
                    </h5>
                </div>

                <div class="col-2 ">
                    <a class="btn_c" href="#">
                        ASK AN EXPERT
                    </a>
                </div>
            </div>
        </section>

        <section id="challenge" class="row text-center justify-content-center p-5">
            <div class="col-10 d-flex flex-column align-items-center">

                <!-- title section -->
                <div class="col-12">
                    <h5>GLOBAL CHALLENGE WORLD CLASS RESPONSE</h5>
                </div>

                <!-- linea decorativa -->
                <div class="col-3 p-4">
                    <hr>
                </div>

                <div class="col-12 d-flex g-3">

                    <div class="col-4">
                        <span>OUR PEOPLE</span>
                    </div>

                    <div class="col-4">
                        <span>OUR PEOPLE</span>
                    </div>

                    <div class="col-4">
                        <span>OUR PEOPLE</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="envato" class="row text-center justify-content-center p-5 bg_third">
            <div class="col-10">

            </div>
        </section>
    </div>
</template>

<script>
export default {
    data(){
        return{
            members:[
                {name: 'Deborah Brown',img: '@/assets/img/column1-image1.jpg'},
                {name: 'Allen Lucas',img: '@/assets/img/column1-image2.jpg'},
                {name: 'Muriel Potter',img: '@/assets/img/column1-image3.jpg'},
                {name: 'Ken Douglas',img: '@/assets/img/column1-image4.jpg'},
                {name: 'Loretta Harris',img: '@/assets/img/column1-image5.jpg'},
                {name: 'Phil Russel',img: '@/assets/img/column1-image6.jpg'}
            ],

            practices:[
                {area: 'tax Litigation',img:'@/assets/img/column2-image1.jpg'},
                {area: 'Aquisitions',img:'@/assets/img/column2-image2.jpg'},
                {area: 'Financial Advice',img:'@/assets/img/column2-image3.jpg'},
                {area: 'International',img:'@/assets/img/column2-image4.jpg'},
                {area: 'Oil and Gas',img:'@/assets/img/column2-image5.jpg'},
                {area: 'Capital Markets',img:'@/assets/img/column2-image6.jpg'}
            ],

            posts:[
                {title: 'Low Oli Prices', img:'@/assets/img/column3-image1.jpg'},
                {title: 'Cost of Divorce', img:'@/assets/img/column3-image2.jpg'},
                {title: '2015 Tax Laws', img:'@/assets/img/column3-image3.jpg'},
                {title: 'Surveys Matter', img:'@/assets/img/column3-image4.jpg'},
                {title: 'In-House Work', img:'@/assets/img/column3-image5.jpg'},
                {title: 'Obama Care', img:'@/assets/img/column3-image6.jpg'}
            ]
        };
    }
}
</script>


<style lang="scss" scoped>
@import '@/assets/scss/style.scss';

.border_t{
    border-top: 3px green solid;

    .bg_first{
    background-color: $col-one;
    border: 1px solid $col-four;

        a{
        background-color: $med-two;
        }
    }
}

#ask{
color:$col-one;
    .btn_c{
        background-color: $my-col;
    }
}

#challenge{
    hr{
        color:  $med-five;
    }
}

#envato{
}
</style>