<script>
import FumettiComp from './FumettiComp.vue'

export default {
    name: "MainComp",
    components: {
        FumettiComp
    },
    data() {
        return {
            articoli: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
}
</script>

<template>
    <div class="content">
        <div id="jumbo"></div>

        <div class="container">

            <div id="serie">
                <span>current series</span>
            </div>

            <div id="cont-fumetti">

                <FumettiComp v-for="(element, index) in articoli" :key="index" :Fumetti="element" />

            </div>

            <div id="load-cont">
                <div>
                    <span class="white">load more</span>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.content {
    margin-top: 3px;
    background-color: black;

    #jumbo {

        background-image: url("/img/jumbotron.jpg");
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        height: 400px;
    }

    .container {
        margin: 0 auto;
        width: 80%;
        padding: 30px 0;
        display: flex;
        flex-direction: column;

        #serie {
            background-color: rgb(2, 130, 249);
            padding: 10px;
            max-width: 200px;
            margin-top: -40px;

            span {
                color: white;
                text-transform: uppercase;
                font-weight: bold;

            }
        }

        #cont-fumetti {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            margin-top: 100px;
        }

        #load-cont {
            display: flex;
            justify-content: center;
            align-items: center;

            div {
                background-color: rgb(2, 130, 249);
                padding: 10px;
                padding-inline: 30px;
                font-weight: bold;
            }
        }
    }
}
</style>