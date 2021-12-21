<template>
    <div class="comic">
        <img :src="objectComic.thumb" :alt="objectComic.series">
        <span class="comic-title">
            {{objectComic.series}}
        </span>
    </div>
</template>
<script>
export default {
    name:'SingleComic',
    props: ['objectComic']
}
</script>
<style lang="scss" scoped>
.comic{
    width: calc(( 100% / 6 ) - 15px) ;
    padding: 15px;
    
        .comic-title{
            margin-top: 20px;
            display: block;
            color:white;
            font-size: 20px;
            
        }
}
</style>