<template>
    <div class="d-flex m-0 bg ">
        <ul v-for="(link,index) in links" :key="index" class="" >
            <li class=" col text-uppercase bold fs-4 text-white">{{ link.title }}</li>
            <li v-for="(item,index) in link.links">
                <a :href="item.link">{{ item.text }}</a>
            </li>
        </ul>
        <div>
            <img src="public/img//dc-logo-bg.png" alt="dc-logo-bg">
        </div>
    </div>
</template>

<script>
import { footerLinks } from '../assets/dat/data';

    export default {
        name: 'FooterLinks',
        data() {
            return {
                links : footerLinks,
            }
        }
    }
</script>

<style lang="scss" scoped>

ul{
    list-style: none;
}
.bg{
    background: url('public/img//footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

</style>