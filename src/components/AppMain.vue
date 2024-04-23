<script>
import SectionCompany from './SectionCompany.vue';
import SectionGaming from './SectionGaming.vue';
import SectionStreaming from './SectionStreaming.vue';
import SectionMatch from './SectionMatch.vue';
import SectionBest from './SectionBest.vue';


export default{
    components: {
        SectionCompany,
        SectionGaming,
        SectionStreaming,
        SectionMatch,
        SectionBest
    }
}

</script>

<template>
<SectionCompany/>
<SectionGaming/>
<SectionStreaming/>
<SectionMatch/>
<SectionBest/>

</template>

<style lang="scss" scoped>
</style>