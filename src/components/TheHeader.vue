<script>
export default {
    name: "TheHeader",
    data() {
        return {
            navLinks: [
                {
                    label: 'caracters',
                    link: '#'
                },
                {
                    label: 'home',
                    link: '#'
                },
                {
                    label: 'movies',
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
                    label: 'collectibles',
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
    width: 60%;
}

.item {
    font-size: 15px;
    list-style: none;
    margin: 10px;
    display: inline-block;
    border-bottom: 5px solid transparent;
    padding: 24px 0;



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