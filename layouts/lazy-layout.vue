<template>
    <div>
        <h1 class="test-style">Color</h1>
        <nuxt/>
    </div>
</template>

<script>
    let moment = () => import('moment-timezone'); // Improved performance
    const created = async () => {
        moment = await moment();
    }
    created()

    export default {
    }
</script>

<style lang="scss" scoped>
    .test-style {
        color: red;
    }
</style>
