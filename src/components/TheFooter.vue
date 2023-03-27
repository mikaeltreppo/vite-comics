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
                } 
        ],
        navLinksThree:[{
            
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
    <h3>DC</h3>
        <ul> 
            <li v-for="item in navLinksThree">
            {{ item.label }}</li>
        </ul>
  </div>
  <div>
    <h3>DC</h3>
        <ul> 
            <li v-for="item in navLinksTwo">
            {{ item.label }}</li>
        </ul>
  </div>
    </div>
</div>
<div class="downFooter">
    <div class="containerTwo">
      <button class="button"><h3>SIGN-UP NOW</h3></button>
      <div class="social">
        <h4>FOLLOW US</h4>
        <img class='socials' src="../assets/img/footer-facebook.png" alt="">
        <img class='socials' src="../assets/img/footer-twitter.png" alt="">
        <img class='socials' src="../assets/img/footer-periscope.png" alt="">
        <img class='socials' src="../assets/img/footer-pinterest.png" alt="">
        <img class='socials' src="../assets/img/footer-youtube.png" alt="">
      </div>
    </div>
</div>

   
</template>

<style scoped>
h4{
    font-weight: bold;
    color: blue;
    margin-right: 10px;
}
.social{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.button{
    display: flex;
    justify-content: center;
    align-items: center;
    border: 2px solid blue;
    padding: 5px;
    background-color: transparent;
    color: white;
}
.button h3{
    margin-right: 0;
}
h3{
    color: white;
    display: inline-block;
    padding: 8px 0;
    margin-right: 20px;
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
.containerTwo{
    width: 80%;
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.socials{
    margin: 5px;
}
.upFooter{
    height: 265px;
    background-image: url('../assets/img/dc-logo-bg.png'), url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat, no-repeat;
    background-size: 30%, 100%;
    background-position: right  , center ;

}
.downFooter{
    background-color: rgb(48, 48, 48);
    height: 70px;
    display: flex;
    align-items: center;


}
</style>