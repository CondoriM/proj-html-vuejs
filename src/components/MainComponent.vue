<template>
    <div class="container-fluid">
        <div class="row text-center justify-content-center p-5 bg_second">
            <div class="col-10 d-flex justify-content-center">

                <!-- ciclo per creare le card in modo dinamico -->
                <div class="col-4 p-4 bg_first" v-for="(col,index) in 3" :key="col + index">
                    <h5>WHO WE  ARE</h5>
                    <p class="mb-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis, ab.</p>
                    <a href="#">LEARN MORE</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import '@/assets/scss/style.scss';

.bg_first{
    background-color: white;
    border-top: 3px green solid;
    border-left: 2px greenyellow solid;
    border-bottom: 2px greenyellow solid;

}

.bg_second{
    background-color: grey;
}

a{
    text-decoration: none;
    color: white;
    padding: 0.5rem;
    background-color: black;
}
</style>