<script>
export default {
    name: 'CardSquareImg',
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div class="box-square">
            <img class="img-square" :src="img" :alt="title">
        </div>
        <h4 class="img-title">{{ title }}</h4>
    </div>
</template>

<style lang="scss" scoped>
.card {
    .box-square {
        width: 100%;
        padding-bottom: 100%;
        position: relative;

        .img-square {
            position: absolute;
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }

    .img-title { 
        font-size: 0.9rem;
        font-weight: 400;
        margin-top: 1.25rem;
        overflow-wrap: break-word;
    }
}
</style>