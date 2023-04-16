<template>
    <div class="cards bg-black">
        <div>
            <ul class="d-flex flex-wrap bg-black text-white">
                <li v-for="(card, index) in cards" :key="index" class="text-uppercase ">
                        <img :src="card.thumb" :alt="card.series" class="img-fluid">
                        <p>{{ card.price }}</p>
                        <a href="#"> {{ card.series }}</a>
                        <p>{{ card.type }}</p>
                </li>
        </ul>
        </div>
    </div>
    
</template>

<script>
import { heros } from '../assets/dat/data';

    export default {
        name: 'CardDc',
        data(){
        return{
            cards : heros,
        }
    }
}
</script>

<style lang="scss" scoped>
ul{
    list-style: none;
}
li{
    padding: 50px;
    width: calc(100% / 6);
}
.cards{
    height: 800px;
}
img{
    min-width: 100%;
    max-height: 200px;
    object-fit: contain;
}

</style>