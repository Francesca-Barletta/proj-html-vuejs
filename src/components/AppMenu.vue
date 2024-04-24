<script>
</script>

<template>
    <ul class="menu">
        <li><a href="#">HOME</a></li>
        <li><a href="#">PAGES</a></li>
        <li><a href="#">TOURNAMENT</a></li>
        <li><a href="#">SHOP</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">CONTACT</a></li>
    </ul>
</template>
<style lang="scss" scoped>
.menu{
    display: flex;
    align-items: center;
    color: white;
    gap: 27px;
    li{
        &:hover{
            color:#05CC7C;
        }
    }
    img{
        width:10px;
        margin-left:1px;
        transform: translatey(10%);
        &:hover{
            fill:#05CC7C;
        }
    }
}
</style>