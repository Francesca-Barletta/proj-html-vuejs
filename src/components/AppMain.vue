<script>
import SectionCompany from './SectionCompany.vue';
import SectionGaming from './SectionGaming.vue';
import SectionStreaming from './SectionStreaming.vue';
import SectionMatch from './SectionMatch.vue';
import SectionBest from './SectionBest.vue';
import SectionTeam from './SectionTeam.vue';
import SectionClient from './SectionClient.vue';



export default{
    components: {
        SectionCompany,
        SectionGaming,
        SectionStreaming,
        SectionMatch,
        SectionBest,
        SectionTeam,
        SectionClient
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
<SectionClient/>

</template>

<style lang="scss" scoped>
</style>