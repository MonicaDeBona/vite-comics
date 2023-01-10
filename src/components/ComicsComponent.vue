<script>
    export default {
        name: 'ComicsComponent',
        props: [
            'imagePath',
            'serie',
            'dcPrice',
            'dcType'
        ],
    }
</script>

<template>
    <div class="comic-card">
        <div class="card-container">
            <span class="hover"> {{ dcType }}  {{ dcPrice }}</span>
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
        text-transform: uppercase;
    }

    .card-container {
        width: 180px;
        height: 180px;
        overflow: hidden;
        position: relative;

        img {
            width: 100%;
        }
    }

    .hover {
        position: absolute;
        background-color: #535353b6;
        color: rgb(255, 255, 255);
        text-align: center;
        width: 100%;
        padding: .8rem;
        display: none;
    }

    .card-container:hover .hover  {
        display: block;
    }

    h4 {
        color: $white-color;
        font-weight: 400;
        padding: 1rem 0 3rem 0;
    }
</style>