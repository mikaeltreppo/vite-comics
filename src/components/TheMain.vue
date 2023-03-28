<script>
import TheCard from './TheCard.vue'

export default {
    components:{
        TheCard
    },
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    label: 'DIGITAL COMICS',
                    link: '../assets/img/buy-comics-digital-comics.png'
                },
                {
                    label: 'DC MERCHANDISE',
                    link: '#'
                },
                {
                    label: 'SUBSCRIPTION',
                    link: '#'
                },
                {
                    label: 'COMIC SHOP LOCATION',
                    link: '#'
                },
                {
                    label: 'DC POWER VISA',
                    link: '#'
                }


            ],
        };
    },
};
</script>

<template>
   
        <div class="hero"></div>
        <div class="blackbar">
        <div class="absolute"> CURRENT SERIES</div>
           <div class="container one"><TheCard></TheCard></div>
        </div>

        <div class="bluebar">
            <div class="container">
            <ul class="listItem">
                <li class="item" v-for="item in navLinks">
                    {{ item.label }}
                </li>
            </ul>
        </div>

     
    </div>
</template>

<style scoped>
.hero{
    background-size: 100%;
    background-repeat: no-repeat;
    background-position-x: center;
    height: 300px;
    background-image: url('../assets/img/jumbotron.jpg');
}
.container{
  width: 80%;
  margin: auto;

}
.container.one{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}
.listItem{
    display: flex;
    align-items: center;
    justify-content: space-between;

}
.item{
    display: flex;
}
.bluebar { 
    background-color:rgb(2, 130, 249);
    height: 80px;
    width: 100%;
    display: flex;
    align-items: center;

}
.absolute{
    position: absolute;
    top: -10px;
    left: 150px;
   display: inline-block;
   background-color: rgb(2, 130, 249);
   color:white;
   font-weight: bolder;
   padding: 5px;
}

.blackbar {
    background-color: black;
position: relative;
    color: wheat;
}
</style>