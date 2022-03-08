<template>
    <footer class="footer">
        <div class="footer__link">
            <div class="container">
                <ul class="nav__menu">
                    <li>
                        <h4>DC Comics</h4>
                        <ul class="nav__link">
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
                    </li>
                    <li>
                        <h4>Shop</h4>
                        <ul class="nav__link">
                            <li>
                                <a href="#">Shop DC</a>
                            </li>
                            <li>
                                <a href="#">Shop DC Collectibles</a>
                            </li>
                        </ul>
                    </li>
                    <li>
                        <h4>DC</h4>
                        <ul class="nav__link">
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
                                <a href="#">Subscriptions</a>
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
                    </li>
                    <li>
                        <h4>Sites</h4>
                        <ul class="nav__link">
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
                                <a href="#">DC Power Visa</a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>

        <div class="footer__social">
            <div class="container">

            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'PageFooter'
}
</script>

<style lang="scss" scoped>
.footer {

    .footer__link {
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 30px 10px 50px;

        .nav__menu {
            display: flex;
            flex-direction: column;
            flex-wrap: wrap;
            height: 280px;
            width: 380px;
            gap: 10px;
            list-style: none;
            
            h4 {
                text-transform: uppercase;
                color: white;
                margin-bottom: 15px;
            }

            .nav__link {
                margin-bottom: 15px;
                list-style: none;

                a {
                    color: #626F7C;
                    text-decoration: none;
                    font-size: 0.7rem;
                }
            }
        }

    }

    .footer__social {
        background-color: var(--app-heavy-grey);
        min-height: 100px;
    }
}
</style>