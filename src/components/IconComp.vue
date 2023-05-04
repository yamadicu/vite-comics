<script>
export default {
    name: "IconComp",
    data() {
        return {
            icons: [
                {
                    nome: "digital comics",
                    path: "buy-comics-digital-comics.png"
                }, {
                    nome: "dc merchandise",
                    path: "buy-comics-merchandise.png"
                }, {
                    nome: "subscription",
                    path: "buy-comics-subscriptions.png"
                }, {
                    nome: "comics shop location",
                    path: "buy-comics-shop-locator.png"
                }, {
                    nome: "dc power visa",
                    path: "buy-dc-power-visa.svg"
                },
            ]
        }
    }
}
</script>

<template>
    <div id="bg-blue">
        <div class="merch">
            <ul>
                <li v-for="(element, index) in icons" :key="index">
                    <img :src="`/img/${element.path}`" alt="nome icona">
                    <span class="icon-text white">{{ element.nome }}</span>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
#bg-blue {
    background-color: rgb(2 130 249);
    padding: 30px 0;

    .merch {
        margin: 0 auto;
        width: 80%;

        ul {
            display: flex;
            align-items: center;
            justify-content: space-around;

            li {
                display: flex;
                align-items: center;
                list-style: none;

                img {
                    height: 70px;
                    margin-right: 10px;
                }
            }
        }
    }
}
</style>