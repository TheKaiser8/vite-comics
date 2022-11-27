<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            socialList: [
                {
                    img: 'src/assets/img/footer-facebook.png',
                    name: 'Logo Facebook'
                },
                {
                    img: 'src/assets/img/footer-twitter.png',
                    name: 'Logo Twitter'
                },
                {
                    img: 'src/assets/img/footer-youtube.png',
                    name: 'Logo YouTube'
                },
                {
                    img: 'src/assets/img/footer-pinterest.png',
                    name: 'Logo Pinterest'
                },
                {
                    img: 'src/assets/img/footer-periscope.png',
                    name: 'Logo Periscope'
                }
            ]
        }
    }
}
</script>

<template>
    <section id="footer-bottom">
        <div class="container">
            <div class="btn-box">
                <button class="btn btn-secondary">SIGN-UP NOW!</button>
            </div>
            <div class="social-box">
                <strong class="social-box__text">FOLLOW US</strong>
                <a href="#" v-for="item in socialList" @click.prevent>
                    <img :src="item.img" :alt="item.name">
                </a>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#footer-bottom {
    background-color: var(--secondary-bg-color);
    padding: 1.875rem 0;
    color: var(--first-text-color);
    
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .btn {
            border: none;
            font-size: inherit;
            background-color: transparent;
            cursor: pointer;
        }
        .btn-secondary {
            border: .125rem solid var(--primary-color);
            padding: 1rem .875rem;
            color: inherit;
            transition: transform 0.5s;

            &:hover {
                transform: scale(1.2);
            }
        }
        .social-box {
            display: flex;
            align-items: center;

            .social-box__text {
                color: var(--primary-color);
                font-size: 1.1rem;
                margin-right: 1.5rem;
            }

            a:not(:last-child) {
                margin-right: 1rem;
            }
        }
    }
}
</style>