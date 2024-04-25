<script>
import data from '../assets/db.json'
import AppMenu from './AppMenu.vue';
import SocialMenu from './SocialMenu.vue'
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
    <div class="section-header">
        <div class="container">
            <div class="row navbar">
                <img class="logo" src="/img/menulogo.png" alt="">
                <ul class="menu">
                    <li v-for="(link, i) in menu" :key="i">
                    <AppMenu :item="link"/>
                    </li>
                </ul>
                <ul class="tools">
                    <li class="round"><img  src="/img/image(1).svg" alt=""></li>
                    <li class="round"><img  src="/img/image(3).svg" alt=""></li>
                </ul>
            </div>
        </div>
        <div class="container-lg">
            <div class="row hero-section">
                <ul>
                 <SocialMenu/>
                </ul>
                <div class="hero">
                    <h4>WELCOME TO RAXG</h4>
                    <h1>ARE YOU READY FOR YOUR NEXT CHALLENGE?</h1>
                    <ul class="buttons">
                        <li><button class="big">Read more<img src="/img/image(8).svg" alt=""></button></li>
                        <li><button class="round"><img src="/img/image(9).svg" alt=""></button></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="container relative">
            <div class="row-pictures">
                <div class="box"><img src="/img/1.png" alt=""></div>
                <div class="box"><img src="/img/2.png" alt=""></div>
                <div class="box"><img src="/img/3.png" alt=""></div>
                <div class="box"><img src="/img/4.png" alt=""></div>
                <div class="box"><img src="/img/5.png" alt=""></div>
                <div class="box"><img src="/img/6.png" alt=""></div>
            </div>
        </div>
    </div>

</template>

<style lang="scss"scoped>
.section-header{
    background-image:url(/img/banner1.png);
    background-size: cover;
    height: 900px;
}
.container-lg{
    width: 1600px;
    margin: 0 auto;
}
.relative{
    position:relative;
}
.row{
    display:flex;
    align-items: center;
}
.navbar{
    height: 70px;
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
    img{
        width:10px;
        margin-left:1px;
        transform: translatey(10%);
        &:hover{
            fill:#05CC7C;
        }
    }
}
.logo{
   height: 70px;
   width: 196px;
   margin-top: 10px;
}
.tools{
    display: flex;
    align-items: center;
    gap: 27px;
    .round{
        width:50px;
        aspect-ratio: 1/1;
        border-radius: 9999px;
        display:flex;
        align-items: center;
        justify-content: center;
        background-color: white;
        img{
            width: 20px;
            aspect-ratio:1/1;
        }
    }

 
}
.hero-section{
    margin-top:215px;
 
}
.hero{
    text-align: center;
    width: 986px;
    margin: 0 auto;
    h4{
        color: #05CC7C;
        margin-bottom: 35px;
    }
    h1{
        color: white;
        font-size: 65px;
    }
}
.buttons{
    display:flex;
    justify-content: center;
    gap: 17px;
    margin-top: 50px;
    button{
        cursor:pointer;
        border: none;
        background-color:#05CC7C;
        height: 55px;
        color:#202046;
        font-size:16px;
        font-weight: 700;
    
    }
    .big{
        padding: 0 32px;
        border-radius:4px;
        display:flex;
        align-items: center;
        gap:10px;
        img{
            width: 20px;
            aspect-ratio:1/1;
        }
        &:hover{
            background-color:#202046;
            color:#05CC7C;
            border: 1px solid #05CC7C;
            img{
                filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
            }
            }
    }
    .round{
        aspect-ratio: 1/1;
        border-radius: 9999px;
        display:flex;
        align-items: center;
        justify-content: center;

        img{
            width: 20px;
            aspect-ratio:1/1;
            transform:translateX(10%);
        }
        &:hover{
            background-color:#202046;
            color:#05CC7C;
            border: 1px solid #05CC7C;
            img{
                filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
            }
            }
    }
}
.row-pictures{
    width: 100%;
    height: 235px;
    background-color: #202046;
    display:flex;
    justify-content: space-around;
    align-items: center;
    gap:5px;
    border-radius: 10px;
    padding:0 10px;
    position: absolute;
    top:215px;
    .box{
        width:150px;
        aspect-ratio: 1/1;
        display:flex;
        justify-content: center;
        align-items: center;
        margin:0 30px;
    }
   
}
</style>