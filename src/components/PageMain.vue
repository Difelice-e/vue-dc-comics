<template>
    <main class="main">
        <div class="container">
            <h2>{{ text }}</h2>
        </div>

        <PageBanner />
    </main>
</template>

<script>
import PageBanner from './PageBanner.vue'

export default {
    name: 'PageMain',
    components: {
        PageBanner
    },
    data() {
        return {
            text: '--> Content goes here <--'
        }
    }
}
</script>

<style lang="scss" scoped>
.main {
    background-color: black;
    color: white;
    min-height: 150px;

    h2 {
        line-height: 120px;
        padding: 30px 10px;
    }
}
</style>