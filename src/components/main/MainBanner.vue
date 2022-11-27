<script>
export default {
    name: 'MainBanner',
}
</script>

<template>
    <section id="main-banner">
        <div class="container">
            <div class="card-icon">
                <img class="img-icon" src="../../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="card-icon">
                <img class="img-icon" src="../../assets/img/buy-comics-merchandise.png" alt="DC Merchandise">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="card-icon">
                <img class="img-icon" src="../../assets/img/buy-comics-subscriptions.png" alt="Subscription">
                <span>SUBSCRIPTION</span>
            </div>
            <div class="card-icon">
                <img class="img-icon" src="../../assets/img/buy-comics-shop-locator.png" alt="Shop Locator">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="card-icon">
                <img class="img-icon" src="../../assets/img/buy-dc-power-visa.svg" alt="DC Power Visa">
                <span>DC POWER VISA</span>
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
            min-width: 15%;

            .img-icon {
                max-height: 3.5rem;
                max-width: 3.5rem;
                margin-right: 1rem;
            }
        }
    }
}
</style>