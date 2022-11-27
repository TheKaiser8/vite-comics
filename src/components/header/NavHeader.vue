<script>
export default {
    name: 'NavHeader',
}
</script>

<template>
    <nav class="main-nav">
        <ul>
            <li><a href="#">CHARACTERS</a></li>
            <li><a href="#" class="active">COMICS</a></li>
            <li><a href="#">MOVIES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">GAMES</a></li>
            <li><a href="#">COLLECTIBLES</a></li>
            <li><a href="#">VIDEOS</a></li>
            <li><a href="#">FAN</a></li>
            <li><a href="#">NEWS</a></li>
            <li><a href="#">SHOP</a></li>
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