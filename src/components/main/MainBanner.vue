<script>
export default {
    name: 'MainBanner',
    data() {
        return {
            bannerList: [
                {
                    img: 'src/assets/img/buy-comics-digital-comics.png',
                    title: 'DIGITAL COMICS'
                },
                {
                    img: 'src/assets/img/buy-comics-merchandise.png',
                    title: 'DC MERCHANDISE'
                },
                {
                    img: 'src/assets/img/buy-comics-subscriptions.png',
                    title: 'SUBSCRIPTION'
                },
                {
                    img: 'src/assets/img/buy-comics-shop-locator.png',
                    title: 'COMIC SHOP LOCATOR'
                },
                {
                    img: 'src/assets/img/buy-dc-power-visa.svg',
                    title: 'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<template>
    <section id="main-banner">
        <div class="container">
            <div class="card-icon" v-for="item in bannerList">
                <img class="img-icon" :src="item.img" :alt="item.title">
                <span>{{ item.title }}</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#main-banner {
    background-color: var(--primary-color);
    padding: 3rem 0;
    color: var(--first-text-color);
    font-weight: 500;
    .container {
        display: flex;
        justify-content: space-around;

        .card-icon {
            display: flex;
            align-items: center;
            min-width: 18%;
            padding: 1rem;
            cursor: pointer;

            &:hover {
                background-color: rgba($color: #000000, $alpha: 0.2);
                border-radius: .625rem;
            }

            .img-icon {
                max-height: 3.5rem;
                max-width: 3.5rem;
                margin-right: 1rem;
            }
        }
    }
}
</style>