<template>
    <main class="">
        <div class="jumbotron">
        </div>
        <button class="text-uppercase btn btn-outline-primary btn-primary text-white text-center position-absolute fs-5 m-1">current series </button>
        <div>
            <CardDc/>
        </div>
    </main>
</template>

<script>
import CardDc from './CardDc.vue';
    export default {
        name : 'MainDc',
        components :{
            CardDc
        }
    }
</script>

<style lang="scss" scoped>
.jumbotron{
    background-image: url('public/img//jumbotron.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    height: 500px;

}

</style>