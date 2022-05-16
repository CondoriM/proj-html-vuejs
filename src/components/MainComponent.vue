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

        <!-- sezione envato -->
        <section id="envato" class="row text-center justify-content-center p-5 bg_third">
            <div class="col-10 flex-column">
                <img src="" alt="">
                <span>"We have worked with Avada Law for the past 15 years. As we have grown and evolved, what i have value most about our relationship is that Avada Law knowus and our business"</span>
                <p class="p-3">Nigel Rawlinson • Senior Partner</p>
            </div>
        </section>

        <section id="law" class="row text-center justify-content-center p-5 bg_second">
            <div class="col-10 d-flex justify-content-center">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="row border_t">
                    <div class="col-4 p-4 bg_first" v-for="(col,index) in law" :key="col + index">
                        <img :src="require(`../assets/img/${col.img}`)" alt="">
                        <h5>{{col.title}}</h5>
                        <p class="mb-3">{{col.text}}</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="together" class="row text-center justify-content-center p-5 ">
            <div class="col-10 d-flex flex-column align-items-center">
                <h4>LET'S WORK TOGETHER</h4>

                <!-- linea decorativa -->
                <div class="col-2 p-4">
                    <hr>
                </div>

                <p>We work as a single united team with market leading firms around the world and give our clients the highest quality advice possible.</p>

                <a class="btn_c my-5" href="#">MAKE ENQUIRY</a>
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
            ],

            law:[
                {img: 'law_7.jpg', title: 'INTERNATIONAL',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'},
                {img: 'law_8.jpg', title: 'PARTNERSHIPS',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'},
                {img: 'law_3.jpg', title: 'EXCELLENCE',text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.'}
            ],
        };
    }, 
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
    background-color: $med-two;
    color: $col-one;
    background-image: url('@/assets/img/showeare-parallax.jpg');
    background-position: center;
}

#law{
    img{
        width: 100%;
    }
}

#together{
    background-image: url('@/assets/img/where-we-work-parallax.jpg');
    background-position: center;
    color: $col-one;

    a{
        background-color: $col-tree;
    }
}
</style>