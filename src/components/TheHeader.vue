<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    label: 'CHARACTERS',
                    link: '#'
                },
                {
                    label: 'HOME',
                    link: '#'
                },
                {
                    label: 'MOVIES',
                    link: '#'
                },
                {
                    label: 'TV',
                    link: '#'
                },
                {
                    label: 'GAMES',
                    link: '#'
                },
                {
                    label: 'COLLECTIBLES',
                    link: '#'
                },
                {
                    label: 'VIDEO',
                    link: '#'
                },
                {
                    label: 'FAN',
                    link: '#'
                },
                {
                    label: 'NEWS',
                    link: '#'
                },
                {
                    label: 'SHOP',
                    link: '#'
                }

            ],
        };
    },
};
</script>

<template>
    <header>
        <div class="container">
            <div class="rigthPart">
                <img class='logoHeader' src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="leftPart">
                <ul class="listLeft">
                    <li class="item" v-for="Item in navLinks">
                        {{ Item.label }}</li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped>
.container {
    width: 80%;
    display: flex;
    margin: auto;
}

header {
    height: 80px;
    background-color: rgb(255, 255, 255);
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.listLeft {
    display: flex;
    justify-content: space-around;

}

.leftPart {
    display: flex;
    align-items: center;
    width: 50%;
}

.item {
    font-size: 15px;
    list-style: none;
    margin: 5px;
    display: inline-block;
    border-bottom: 5px solid transparent;
    padding: 25px 0;



}

.item:hover {
    border-bottom: 5px solid rgb(104, 104, 208);
}

.logoHeader {
    height: 60px;
    margin: 10px;
}

.rigthPart {
    width: 40%;
}</style>