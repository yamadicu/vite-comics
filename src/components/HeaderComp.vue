<script>
export default {
    name: "HeaderComp",
    data() {
        return {
            linkBar: [
                {
                    url: '/',
                    name: 'characters',
                    stato: false
                }, {
                    url: '/',
                    name: 'comics',
                    stato: true
                }, {
                    url: '/',
                    name: 'movies',
                    stato: false
                }, {
                    url: '/',
                    name: 'tv',
                    stato: false
                }, {
                    url: '/',
                    name: 'games',
                    stato: false
                }, {
                    url: '/',
                    name: 'collectibles',
                    stato: false
                }, {
                    url: '/',
                    name: 'videos',
                    stato: false
                }, {
                    url: '/',
                    name: 'fans',
                    stato: false
                }, {
                    url: '/',
                    name: 'news',
                    stato: false
                }, {
                    url: '/',
                    name: 'shop',
                    stato: false
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <nav>
            <img src="/img/dc-logo.png" alt="logo dc">
            <ul>
                <li v-for="(element, index) in linkBar" :key="index" :class="element.stato ? 'active' : ''">
                    <a href="element.url">{{ element.name }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
header {
    height: 100px;

    nav {
        margin: 0 auto;
        width: 80%;
        display: flex;
        align-items: center;
        justify-content: space-between;

        img {
            height: 80px;
        }

        ul {
            display: flex;

            li {
                list-style: none;
                margin: 0 10px;
                line-height: 100px;

                a {
                    text-decoration: none;
                    color: black;
                    text-transform: uppercase;
                    font-weight: bold;
                    font-size: 0.8rem;
                }

                &.active {
                    border-bottom: 3px solid rgb(2 130 247);
                }

                &.active a {
                    color: rgb(2 130 247);
                }
            }
        }
    }
}
</style>
