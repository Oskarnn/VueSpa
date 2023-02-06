<script setup>
    import HeroImage from '../components/HeroImage.vue'
    import SpaOffers from '../components/SpaOffers.vue'
</script>

<template>
    <!-- Lägger in komponent HeroImage -->
    <HeroImage />
    <!-- Textinterpolering -->
    <h1 class="title">{{ message }}</h1>
    <div id="offers">
        <div class="container text-center">
            <div class="row align-items-start">
                <SpaOffers />
                <SpaOffers />
                <SpaOffers />
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                message: 'Vilket paket önskas?'
            }
        }
    }
</script>
<style scoped>
    #offers {
        display: flex;
        justify-content: center;
        margin-top: 10vh;
        margin-bottom: 10vh;
    }
    .title,
    h1 {
        display: flex;
        justify-content: center;
        margin-top: 10vh;
    }
</style>
