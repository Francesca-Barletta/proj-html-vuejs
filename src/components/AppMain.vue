<script>
import SectionCompany from './SectionCompany.vue';
import SectionGaming from './SectionGaming.vue';
import SectionStreaming from './SectionStreaming.vue';
import SectionMatch from './SectionMatch.vue';


export default{
    components: {
        SectionCompany,
        SectionGaming,
        SectionStreaming,
        SectionMatch
    }
}

</script>

<template>
<SectionCompany/>
<SectionGaming/>
<SectionStreaming/>
<SectionMatch/>

</template>

<style lang="scss" scoped>
</style>