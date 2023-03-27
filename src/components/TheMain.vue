<script>
export default {
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
   
        
        <div class="blackbar">
           <div class="container">  <h3>Content goes here</h3>   </div>
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
.container{
  width: 80%;
  margin: auto;
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
    background-color: blue;
    height: 80px;
    width: 100%;
    display: flex;
    align-items: center;

}

.blackbar {
    background-color: black;
    height: 70px;
    color: wheat;
}
</style>