<script>
export default {
    props: {
        item: Object
    }

}
</script>

<template>

    <a :href="item.url">{{ item.text }}</a>

</template>
<style lang="scss" scoped>

</style>