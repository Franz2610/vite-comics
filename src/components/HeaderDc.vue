<template>
    <div>
        <header class="row justify-content-between align-items-center h-100 container mx-auto">
            <div class="col-2 p-2">
                <img class="img-fluid" src="../assets/vue-dc-comics-1/img/dc-logo.png" alt="Dc Logo">
            </div>
            <div class="col-10 p-2 d-flex justify-content-end h-100">
                <ul class="d-flex justify-content-center gap-3 list-unstyled flex-wrap m-0 p-0 h-100">
                    <li v-for="(link, index) in links" :key="index" :class="{active : link.active}" class="text-uppercase">
                        <a href="#">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </header>
    </div>
</template>

<script>
    import {headerLinks} from '../assets/dat/data.js';
    export default {
        name:'HeaderDc',
        data(){
            return {
                links: headerLinks
            }
        }

    }
</script>

<style lang="scss" scoped>

</style>