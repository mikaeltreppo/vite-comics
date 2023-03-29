<template>
     <div v-for="card in carte" class="card">
        <img :src="card.thumb" alt="">
        <span>{{ card.series }}</span>
    </div>
</template>

<style></style>
<script>
export default {
    name: 'TheSingleCard',
    props:{
       carte: Array
        
    }
}


</script>

