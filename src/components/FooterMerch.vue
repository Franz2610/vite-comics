<template>
    <div class="bg-primary">
        <div class="container py-4">
            <div class="row justify-content-center gap-2">
                <div v-for="(image, index) in images" :key="index" class="col d-flex justify-content-center align-items-center gap-1">
                    <img class="img-fluid" :src="'public/img/' + image.img" :alt="image.alt">
                    <p class="m-0 text-white text-uppercase fs-5">{{ image.name }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import { footerMerchImg } from '../assets/dat/data.js';
    export default {
        name: 'FooterMerch',
        data() {
            return {
                images: footerMerchImg,
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>