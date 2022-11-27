<script>
export default {
    name: 'NavHeader',
    data() {
        return {
            currentActiveIndex: 0,
            mainNavList: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FAN',
                'NEWS',
                'SHOP'
            ]
        }
    },
    methods: {
        onClickLinkNav(i) {
            this.currentActiveIndex = i;
        }
    }
}
</script>

<template>
    <nav class="main-nav">
        <ul>
            <li v-for="(item, index) in mainNavList" @click="onClickLinkNav(index)">
                <a href="#" :class="{ active : index === currentActiveIndex }">{{ item }}</a>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
.main-nav {
    ul {
        display: flex;
        list-style: none;

        li {
            &:last-child{
                margin-right: -1rem;
            }
            a {
                text-decoration: none;
                color: currentColor;
                font-weight: 500;
                padding: 1rem;

                &.active {
                    color: var(--primary-color);
                    position: relative;

                    &::after {
                        content: '';
                        display: block;
                        position: absolute;
                        bottom: -55%;
                        left: 1rem;
                        width: calc(100% - 2rem);
                        height: 4px;
                        background-color: var(--primary-color);
                    }
                }
            }
        }
    }
}

</style>