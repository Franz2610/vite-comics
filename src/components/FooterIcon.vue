<template>
    <div class="bg-black">
        <div class="container py-4 d-flex justify-content-between align-items-center">
            <div>
                <button class="text-uppercase">sign-up now!</button>
            </div>
            <div class="d-flex align-items-center gap-3">
                <h3 class="text-primary m-0 text-uppercase bold fs-6">follow us</h3>
                <div class="d-flex gap-3">
                    <img src="/img/footer-facebook.png" alt="facebook">
                    <img src="/img/footer-twitter.png" alt="twitter">
                    <img src="/img/footer-youtube.png" alt="youtube">
                    <img src="/img/footer-pinterest.png" alt="pinterest">
                    <img src="/img/footer-periscope.png" alt="periscope">
                </div>
            </div>
           
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterIcon',
        
    }
</script>

<style lang="scss" scoped>
button{
    border: 1px solid blue;
    background-color: transparent;
    color: white;
    font-size: 12px;
    padding: 10px;
    &:hover{
        background-color: blue;
    }
}
</style>