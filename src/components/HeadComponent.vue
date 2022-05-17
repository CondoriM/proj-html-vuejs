<template>
    <div class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-12 col-xxl-6 p-1 d-flex align-items-center">
                <div class="col-8 text-center">
                    <p class="t_two ">Avada & Associates legal team announce deal to open up oil & gas</p>
                </div>

                <div class="col-sm-2 col-lg-2 text-end">
                    <div class="col-7 d-flex gap-1 text-center">
                        <div class="col-3 social" v-for="(social,index) in socials" :key="index">
                            <img :src="require(`../assets/img/${social.img}`)" alt="">
                        </div>                            
                    </div>
                </div>
            </div>

            <div class="col-12 p-0">
                <img class="jumbo" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default{
    name: 'HeadSite',

    data(){
        return{
            socials:[
                {img:'facebook.png'},
                {img:'twitter.png'},
                {img:'instagram.png'},
                {img:'youtube.png'}
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/assets/scss/style.scss';

.social img{
    width: 100%;
    filter: grayscale(100%);
}
</style>