<script>

</script>

<template>
    <div class="section-header">
        <div class="container">
    <div class="row">
        <img class="logo" src="/img/menulogo.png" alt="">
        <ul class="navbar">
            <li>Home</li>
            <li>Pages</li>
            <li>Tournament</li>
            <li>Shop</li>
            <li>Blog</li>
            <li>Contact</li>
        </ul>
        <ul class="tools">
            <li><img src="/img/image(1).svg" alt=""></li>
            <li><img src="/img/image(3).svg" alt=""></li>
        </ul>
    </div>
    
</div>
    </div>

</template>

<style lang="scss">
.section-header{
    background-image:url(/public/img/banner1.png)
}
.container{
    width: 1299px;
    height: 900px;
    margin: 0 auto;
}
.row{
    display:flex;
    justify-content: space-between;
    align-items: center;
    height: 70px;
}
.navbar{
    display: flex;
    align-items: center;
    color: white;
    gap: 27px;
}
.logo{
   height: 70px;
   width: 196px;
   margin-top: 10px;
}
.tools{
    display: flex;
    align-items: center;
    color: white;
    gap: 27px;
    img{
        filter: invert(100%);
        width: 20px;

    }
}
</style>