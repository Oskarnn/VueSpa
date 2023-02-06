<template>
    <!-- Bootstrap card -->
    <div class="col">
        <div class="card" style="width: 18rem">
            <img
                src="../assets/img/laura-chouette-bD4j1V52dx0-unsplash.jpg"
                class="card-img-top"
                alt="bath"
            />
            <div class="card-body">
                <h5 class="card-title">{{ offer.name }}</h5>
                <p class="card-text">
                    {{ offer.including }}
                </p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        offer:{
            required: true,
            type: Object
        }

    }
}
</script>
<style></style>
