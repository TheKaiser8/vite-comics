<script>
export default {
    name: 'MainBanner',
}
</script>

<template>
    <section>
        <div class="container">
            <div class="card">
                <div class="box-icon">
                    <img class="mr-1" src="../../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                </div>
                <span>DIGITAL COMICS</span>
            </div>
            <div class="card">
                <img class="mr-1" src="../../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="card">
                <img class="mr-1" src="../../assets/img/buy-comics-subscriptions.png" alt="Subscription">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="card">
                <img class="mr-1" src="../../assets/img/buy-comics-shop-locator.png" alt="Shop Locator">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="card">
                <img class="mr-1" src="../../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
                <span>DC POWER VISA</span>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: var(--primary-color);
    padding: 3rem 0;
    color: var(--first-text-color);
    font-weight: 500;
    .container {
        display: flex;
        justify-content: space-around;

        .card {
            display: flex;
            align-items: center;

            img {
                max-height: 3.5rem;
                max-width: 3.5rem;
            }
            .mr-1 {
                    margin-right: 1rem;
                }
        }
    }
}
</style>