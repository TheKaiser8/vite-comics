<script>
import MainContent from './MainContent.vue';
import MainBanner from './MainBanner.vue';

export default {
    name: 'AppMain',
    components: {
        MainContent,
        MainBanner
    }
}
</script>

<template>
    <main>
        <MainContent/>
        <MainBanner/>
    </main>
</template>

<style></style>