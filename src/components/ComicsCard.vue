<template>
    <div class="comics">
        <img :src="details.thumb" alt="Comics">
        <h4>{{details.series}}</h4>
    </div>
</template>

<script>
export default {
    name:'ComicsCard',
    props: {
        details: Object
    }
}
</script>

<style scoped lang="scss">
.comics {
    width: calc(100% / 6 - 30px);
    height:180px;
    margin: 10px 15px;
    color: white;
    font-size: 12px;
    text-transform: uppercase ;
    cursor: pointer;
    
    img {
        width: 100%;
        height: 80%;
        object-fit: cover;
        object-position: top ;
    }
}

</style>