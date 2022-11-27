<script>
export default {
    name: 'FooterTop',
}
</script>

<template>
    <section id="footer-top">
        <div class="container">
            <div class="col">
                <h4>DC COMICS</h4>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>
                </ul>
                <h4>SHOP</h4>
                <ul>
                    <li><a href="#">Shop DC</a></li>
                    <li><a href="#">Shop DC Collectibles</a></li>
                </ul>
            </div>
            <div class="col">
                <h4>DC</h4>
                <ul>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div class="col">
                <h4>SITES</h4>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#footer-top {
    background-image: url('../../assets/img/footer-bg.jpg');
    background-size: cover;
    color: var(--first-text-color);

    .container {
        display: flex;
        padding-top: 2.5rem;
        padding-bottom: 3.5rem;
        background-image: url('../../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: right;

        .col {
            margin-right: 1.5rem;
            h4 {
                margin-bottom: 1rem;
            }
            ul {
                list-style: none;
                margin-bottom: 1.3rem;

                a {
                    text-decoration: none;
                    color: var(--second-text-color);
                    font-size: .875rem;
                }
                a:hover {
                    color: var(--first-text-color);
                    transition: 0.2s;
                }
            }
        }
    }
}
</style>