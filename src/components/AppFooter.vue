<script>

</script>

<template>

    <section class="top-footer">
        <div class="my-container">
            <div class="footer-link">
                <ul>
                    <li>
                        <h3>DC COMICS</h3>
                    </li>
                    <li>Charters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                    <li>
                        <h3>SHOP</h3>
                    </li>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>

                <ul>
                    <li>
                        <h3>DC</h3>
                    </li>
                    <li>Term Of Use</li>
                    <li>Privacy Policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>

                <ul>
                    <li>
                        <h3>SITES</h3>
                    </li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="bottom-footer">
        <div class="my-container">
            <div class="bottom-footer-content">
                <div class="sign-up-button">
                <button>SIGN-UP NOW!</button>
                    </div>
                <div class="social">
                    <h3>FOLLOW US</h3>
                    <img src="../assets/imgs/footer-facebook.png" alt="Facebook Logo">
                    <img src="../assets/imgs/footer-twitter.png" alt="Twitter Logo">
                    <img src="../assets/imgs/footer-youtube.png" alt="Youtube Logo">
                    <img src="../assets/imgs/footer-pinterest.png" alt="Pinterest Logo">
                    <img src="../assets/imgs/footer-periscope.png" alt="Periscope Logo">
                </div>
            </div>
        </div>
    </section>
</template>



<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    .top-footer {
        background-image: url(../assets/imgs/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        padding: 3rem;
    }

    .footer-link {
        display: flex;

        ul {
            list-style-type: none;
            padding-right: 3rem;

            li {
                color: #869579;
                padding-bottom: .2rem;
                font-size: .8rem;

                h3 {
                    color: $white-color;
                    padding: .5rem 0;
                }
            } 
        }
    }
    .bottom-footer {
        background-color: $footer-color;
        padding: 2rem;
    }

    .bottom-footer-content {
        display: flex;
        justify-content: space-between;
    }

    .sign-up-button button {
        background-color: transparent;
        border: 2px solid $blue-color;
        padding: .7rem;
        color: $white-color;
        font-weight: 700;
        font-size: 1rem;
    }

    .social {
        display: flex;
        justify-content: space-between;
        flex-basis: 30%;
        align-items: center;

        h3 {
            color: $blue-color;
        }
    }

</style>