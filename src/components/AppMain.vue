<script>
import SectionCompany from './SectionCompany.vue';
import SectionGaming from './SectionGaming.vue';
import SectionStreaming from './SectionStreaming.vue';
import SectionMatch from './SectionMatch.vue';
import SectionBest from './SectionBest.vue';
import SectionTeam from './SectionTeam.vue';


export default{
    components: {
        SectionCompany,
        SectionGaming,
        SectionStreaming,
        SectionMatch,
        SectionBest,
        SectionTeam
    }
}

</script>

<template>
<SectionCompany/>
<SectionGaming/>
<SectionStreaming/>
<SectionMatch/>
<SectionBest/>
<SectionTeam/>

</template>

<style lang="scss" scoped>
</style>