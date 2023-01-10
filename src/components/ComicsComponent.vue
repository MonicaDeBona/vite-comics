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
    <div class="my-container">
        <div class="comic-card">
            {{ imagePath }} -- {{ serie }}
        </div>
    </div>
</template>


<style lang="scss" scoped>

</style>