<script>
export default {
    name: 'FooterTop',
    data() {
        return {
            dcComicsList: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],
            shopList: [
                'Shop DC',
                'Shop DC Collectibles'
            ],
            dcList: [
                'Terms Of Use',
                'Privacy policy (New)',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshops',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            sitesList: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ]
        }
    }
}
</script>

<template>
    <section id="footer-top">
        <div class="container">
            <div class="col">
                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="item in dcComicsList" @click.prevent><a href="#">{{ item }}</a></li>
                </ul>
                <h4>SHOP</h4>
                <ul>
                    <li v-for="item in shopList" @click.prevent><a href="#">{{ item }}</a></li>
                </ul>
            </div>
            <div class="col">
                <h4>DC</h4>
                <ul>
                    <li v-for="item in dcList" @click.prevent><a href="#">{{ item }}</a></li>
                </ul>
            </div>
            <div class="col">
                <h4>SITES</h4>
                <ul>
                    <li v-for="item in sitesList" @click.prevent><a href="#">{{ item }}</a></li>
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