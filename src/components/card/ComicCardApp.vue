<script>
import { info } from 'sass';


export default {
    name:"ComicCardApp",
    props: {
        item: Object
    }
}
</script>

<template>

<div class="item">
    <div>
        <img :src="item.thumb" alt="">
    </div>

    <div class="title">
        {{ item.series }}
    </div>
</div>

</template>


<style lang="scss" scoped>

.item {
    flex-basis: calc((100% / 6) - 10px);
    padding: 20px;
    margin-top: 20px;

    img {
        height: 200px;
        object-fit: contain;
    }
}

.title {
    color: white;
    padding-top: 10px;
}

</style>