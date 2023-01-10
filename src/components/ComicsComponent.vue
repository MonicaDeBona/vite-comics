<script>
    export default {
        name: 'ComicsComponent',
        props: [
            'imagePath',
            'serie'
        ],
    }
</script>

<template>
    <div class="comic-card">
        <div class="card-container">
            <img :src="imagePath" :alt="serie">
        </div>
        <h4> {{ serie }}</h4>
    </div>
</template>


<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
    .comic-card {
        width: calc(100% / 6);
        padding: 1rem;
    }

    .card-container {
        width: 180px;
        height: 180px;
        overflow: hidden;

        img {
            width: 100%;
        }
    }

    h4 {
        color: $white-color;
        font-weight: 400;
        padding: 1rem 0 3rem 0;
        text-transform: uppercase;
    }
</style>