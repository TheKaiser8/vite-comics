<script>
import AppLogo from './AppLogo.vue';
import NavHeader from './NavHeader.vue';

export default {
    name: 'AppHeader',
    components: {
        AppLogo,
        NavHeader
    }
}
</script>

<template>
    <header class="container">
        <AppLogo/>
        <NavHeader/>
    </header>
</template>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 0;
}
</style>
