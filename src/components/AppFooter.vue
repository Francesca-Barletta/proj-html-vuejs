<script>

import data from '../assets/db.json'
import AppMenu from './AppMenu.vue';
import SocialMenu from './SocialMenu.vue';

export default{
    components: {
        AppMenu,
        SocialMenu
    },
    data() {
        return {
             menu: data.menu
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
                    <li v-for="(link, i) in menu" :key="i">
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
                    <SocialMenu/>
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
    
}
</style>
