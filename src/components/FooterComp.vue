<script>
export default {
    name: "FooterComp"
}
</script>

<template>
    <footer>
        <div class="container footer-bg">
            <div class="col-1">
                <div>
                    <ul>
                        <h4 class="white">DC COMICS</h4>
                        <li>
                            <a href="#">Characters</a>
                        </li>
                        <li>
                            <a href="#">Comics</a>
                        </li>
                        <li>
                            <a href="#">Movies</a>
                        </li>
                        <li>
                            <a href="#">TV</a>
                        </li>
                        <li>
                            <a href="#">Games</a>
                        </li>
                        <li>
                            <a href="#">Videos</a>
                        </li>
                        <li>
                            <a href="#">News</a>
                        </li>
                    </ul>
                    <ul>
                        <h4 class="titolo-lista white">SHOP</h4>
                        <li>
                            <a href="#">Shop DC</a>
                        </li>
                        <li>
                            <a href="#">Shop DC Collectibles</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <h4 class="titolo-lista white">DC</h4>
                        <li>
                            <a href="#">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="#">Privacy policy (New)</a>
                        </li>
                        <li>
                            <a href="#">Ad Choices</a>
                        </li>
                        <li>
                            <a href="#">Advertising</a>
                        </li>
                        <li>
                            <a href="#">Jobs</a>
                        </li>
                        <li>
                            <a href="#">Subscription</a>
                        </li>
                        <li>
                            <a href="#">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="#">CPSC Certificates</a>
                        </li>
                        <li>
                            <a href="#">Ratings</a>
                        </li>
                        <li>
                            <a href="#">Shop Help</a>
                        </li>
                        <li>
                            <a href="#">Contact Us</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <ul>
                        <h4 class="titolo-lista white">SITES</h4>
                        <li>
                            <a href="#">DC</a>
                        </li>
                        <li>
                            <a href="#">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="#">DC Kids</a>
                        </li>
                        <li>
                            <a href="#">DC Universe</a>
                        </li>
                        <li>
                            <a href="#">DC Pover Visa</a>
                        </li>
                    </ul>
                </div>

            </div>
            <div>

            </div>
        </div>
        <div id="parte-social">
            <div class="container">
                <a href="#" class="footer-botton">Sign- up now!</a>
                <div id="social">
                    <span id="follow">follow us</span>
                    <img src="/img/footer-facebook.png" alt="social facebook">
                    <img src="/img/footer-twitter.png" alt="social twitter">
                    <img src="/img/footer-youtube.png" alt="youtube logo">
                    <img src="/img/footer-pinterest.png" alt="social pinterest">
                    <img src="/img/footer-periscope.png" alt="periscope logo">
                </div>
            </div>

        </div>
    </footer>
</template>

<style scoped lang="scss">
footer {
    background-image: url('/img/footer-bg.jpg');

    .footer-bg {
        background-image: url('/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-size: 40%;
        background-position: center right;
    }

    .container {
        padding: 30px 0;
        margin: 0 auto;
        width: 80%;
        display: flex;

        div {
            width: 50%;

            h4 {
                text-transform: uppercase;
                margin-bottom: 20px;
            }

            ul {
                li {
                    list-style: none;
                    line-height: 180%;

                    a {
                        text-decoration: none;
                        color: grey;
                    }
                }
            }
        }

        .col-1 {
            display: flex;

            div {
                width: calc(100%/3);
            }
        }
    }

    #parte-social {
        background-color: rgb(48 48 48);

        .container {
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .footer-botton {
            color: white;
            text-decoration: none;
            border: 2px solid rgb(2 130 247);
            padding: 20px;
        }

        #social {
            display: flex;
            align-items: center;

            #follow {
                text-transform: uppercase;
                font-weight: bold;
                margin: 10px;
                color: rgb(2 130 247);
            }
        }
    }
}
</style> 