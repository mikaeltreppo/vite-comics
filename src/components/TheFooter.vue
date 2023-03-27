<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    label: 'Characters',
                    link: '#'
                },
                {
                    label: 'Comics',
                    link: '#'
                },
                {
                    label: 'Movies',
                    link: '#'
                },
                {
                    label: 'tv',
                    link: '#'
                },
                {
                    label: 'games',
                    link: '#'
                },
                {
                    label: 'News',
                    link: '#'
                },
                {
                    label: 'video',
                    link: '#'
                },
                {
                    label: 'fan',
                    link: '#'
                },
                {
                    label: 'news',
                    link: '#'
                },
                {
                    label: 'shop',
                    link: '#'
                }

            ],
        };
    },
};
</script>

<template>
  

<div class="upFooter">
    <div class="container">
        <div>
        <h3>DC COMICS</h3>
        <ul> 
            <li v-for="item in navLinks">
            {{ item.label }}</li>
        </ul>
  </div>
    </div>
</div>
<div class="downFooter">
    <div class="container">
      
    </div>
</div>

   
</template>

<style scoped>
h3{
    color: white;
}
ul{
    color: rgb(168, 159, 159);
    list-style: none;
    font-size: 10px;
}

.container{
    padding: 20px;
    width: 80%;
    margin: auto;
}
.upFooter{
    height: 265px;
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;

}
.downFooter{
    background-color: rgb(48, 48, 48);
    height: 70px;

}
</style>