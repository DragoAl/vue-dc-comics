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
    width: calc(100% / 6 );
 
    

}

</style>