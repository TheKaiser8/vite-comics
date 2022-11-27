<script>
import MainContent from './MainContent.vue';
import MainBanner from './MainBanner.vue';
import AppJumbotron from './AppJumbotron.vue';

export default {
    name: 'AppMain',
    components: {
        AppJumbotron,
        MainContent,
        MainBanner
    }
}
</script>

<template>
    <main>
        <AppJumbotron/>
        <MainContent/>
        <MainBanner/>
    </main>
</template>

<style></style>