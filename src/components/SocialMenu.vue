<script>

</script>

<template>
    <li class="round"><a href="#"><img src="/img/image(4).svg" alt=""></a></li>
    <li class="round"><a href="#"><img src="/img/image(5).svg" alt=""></a></li>
    <li class="round"><a href="#"><img src="/img/image(6).svg" alt=""></a></li>
    <li class="round"><a href="#"><img src="/img/image(7).svg" alt=""></a></li>
</template>
<style lang="scss" scoped>
.round{
        cursor:pointer;
        width:50px;
        aspect-ratio: 1/1;
        border-radius: 9999px;
        display:flex;
        align-items: center;
        justify-content: center;
        background-color: #202046;
        margin-bottom:12px;
    img{
        filter: invert(100%);
        width: 20px;
        transform: translateY(2px);
    }
    &:hover{
        background-color: #05CC7C;
    }
    }
</style>