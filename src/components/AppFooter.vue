<script>
import { store } from '../store.js';
import AppMenu from './AppMenu.vue';

export default{
    components: {
        AppMenu
    },
    data() {
        return {
            store: store,
        }
    }
}
</script>

<template>
<div class="section">
    <div class="bg-overlay">
        <div class="container">
            <div class="row footermenu">
                <img class="logo" src="/img/menulogo.png" alt="">
                <ul class="menu">
                    <li v-for="(link, i) in store.menu" :key="i">
                    <AppMenu :item="link"/>
                    </li>
                </ul>
            </div>
            <hr>
            <div class="flex">
                <div>
                    <span class="white">Copyright RaxG | Designed by</span>
                    <span class="green">NextGenerationDev</span>
                </div>
            
                <ul class="social">
                        <li class="round"><a href="#"><img src="/img/image(4).svg" alt=""></a></li>
                        <li class="round"><a href="#"><img src="/img/image(5).svg" alt=""></a></li>
                        <li class="round"><a href="#"><img src="/img/image(6).svg" alt=""></a></li>
                        <li class="round"><a href="#"><img src="/img/image(7).svg" alt=""></a></li>
                </ul>
            </div>
        </div>

    </div>
</div>
</template>

<style lang="scss"scoped>
.section{
    background-image:url(/img/footer-bg.png);
    background-size: cover;
    .bg-overlay{
        background: rgba(25, 25, 53, 0.7);
    }
    
    
}
.container{
    width: 80%;
    margin: 0 auto;
    height: 370px;
    padding-top: 150px;
    hr{
        color: rgba(255, 255, 255, 0.4);
        margin-bottom: 16px;
    }
}
.row{
    display:flex;
    align-items: center;
    margin-bottom: 22px;
}
.footermenu{
    height: 100px;
    justify-content: space-between;
}
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
}
.logo{
   height: 70px;
   width: 196px;
   margin-top: 10px;
}
.green{
    color: #05CC7C;
}
.white{
    color:white;
}
.flex{
    display:flex;
    justify-content: space-between;
    align-items: center;
}
.social{
    display: flex;
    gap:20px;
    .round{
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
    }
}
</style>
