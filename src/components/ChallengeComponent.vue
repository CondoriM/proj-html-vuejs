<template>
    <div class="container-fluid">
        <section id="challenge" class="row text-center justify-content-center p-5">
            <div class="col-10 col-sm-12 col-xl-8 col-xxl-6 d-flex flex-column align-items-center">

                <!-- title section -->
                <div class="col-12">
                    <h5>GLOBAL CHALLENGE WORLD CLASS RESPONSE</h5>
                </div>

                <!-- linea decorativa -->
                <div class="col-3 p-4">
                    <hr>
                </div>

                <div class="col-12 d-flex gap-3 justify-content-center text-start">

                    <!-- prima colonna "Members" -->
                    <div class="col-4 d-flex flex-column">
                        <span class="fw-bolder">OUR PEOPLE</span>

                        <div class="my_card d-flex my-2 p-3 justify-content-between" v-for="(member,index) in members" :key="index">
                            <div class="col-3">
                                <div class="card rounded-0">
                                    <img :src="require(`../assets/img/${member.img}`)" alt="">
                                </div>
                            </div>

                            <div class="col-8 d-flex align-items-center">   
                                <p class="t_one fw-bolder">{{member.name}}</p>
                            </div>
                        </div>
                    </div>

                    <!-- seconda colonna "Practices" -->
                    <div class="col-4 d-flex flex-column">
                        <span class="fw-bolder">OUR PRACTICE AREAS</span>

                        <div class="my_card d-flex my-2 p-3 justify-content-between" v-for="(practic,index) in practices" :key="index + practic">
                            <div class="col-3">
                                <div class="card rounded-0">
                                    <img :src="require(`../assets/img/${practic.img}`)" alt="">
                                </div>
                            </div>

                            <div class="col-8 d-flex align-items-center">   
                                <p class="t_one fw-bolder">{{practic.area}}</p>
                            </div>
                        </div>
                    </div>

                    <!-- terza colonna "Posts" -->
                    <div class="col-4 d-flex flex-column">
                        <span class="fw-bolder">OUR PUBLICATIONS</span>

                        <div class="my_card d-flex my-2 p-3 justify-content-between" v-for="(post,index) in posts" :key="index">
                            <div class="col-3">
                                <div class="card rounded-0">
                                    <img :src="require(`../assets/img/${post.img}`)" alt="">
                                </div>
                            </div>

                            <div class="col-8 d-flex align-items-center">   
                                <p class="t_one fw-bolder">{{post.title}}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default{
    name:'ChallengeComp',

    data(){
        return{
            members:[
                {name: 'Deborah Brown',img: 'column1-image1.jpg'},
                {name: 'Allen Lucas',img: 'column1-image2.jpg'},
                {name: 'Muriel Potter',img: 'column1-image3.jpg'},
                {name: 'Ken Douglas',img: 'column1-image4.jpg'},
                {name: 'Loretta Harris',img: 'column1-image5.jpg'},
                {name: 'Phil Russel',img: 'column1-image6.jpg'}
            ],

            practices:[
                {area: 'tax Litigation',img:'column2-image1.jpg'},
                {area: 'Aquisitions',img:'column2-image2.jpg'},
                {area: 'Financial Advice',img:'column2-image3.jpg'},
                {area: 'International',img:'column2-image4.jpg'},
                {area: 'Oil and Gas',img:'column2-image5.jpg'},
                {area: 'Capital Markets',img:'column2-image6.jpg'}
            ],

            posts:[
                {title: 'Low Oli Prices', img:'column3-image1.jpg'},
                {title: 'Cost of Divorce', img:'column3-image2.jpg'},
                {title: '2015 Tax Laws', img:'column3-image3.jpg'},
                {title: 'Surveys Matter', img:'column3-image4.jpg'},
                {title: 'In-House Work', img:'column3-image5.jpg'},
                {title: 'Obama Care', img:'column3-image6.jpg'}
            ],
        }
    }
}
</script>

<style lang="scss">
@import '@/assets/scss/style.scss';
</style>
