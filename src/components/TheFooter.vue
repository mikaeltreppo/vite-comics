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
            navLinksTwo:[
                
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

            
        ]
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

        <h3>SHOP</h3>
        <ul> 
            <li v-for="itemTwo in navLinksTwo">
            {{ itemTwo.label }}</li>
        </ul>
  </div>
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
    display: inline-block;
    padding: 8px 0;
}
ul{
    color: rgb(168, 159, 159);
    list-style: none;
    font-size: 10px;
    margin-right: 20px;
}

.container{
    display: flex;
    padding: 10px;
    width: 80%;
    margin: auto;
}
.upFooter{
    height: 265px;
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat, no-repeat;
    background-size: 40%, 100%;
    background-position: 20px 50px, ;

}
.downFooter{
    background-color: rgb(48, 48, 48);
    height: 70px;

}
</style>