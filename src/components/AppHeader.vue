<script>

</script>

<template>
    <div class="section-header">
        <div class="container">
            <div class="row navbar">
                <img class="logo" src="/img/menulogo.png" alt="">
                <ul class="menu">
                    <li><a href="#">Home<img src="/img/image.svg" alt=""></a></li>
                    <li><a href="#">Pages<img src="/img/image.svg" alt=""></a></li>
                    <li><a href="#">Tournament</a></li>
                    <li><a href="#">Shop<img src="/img/image.svg" alt=""></a></li>
                    <li><a href="#">Blog<img src="/img/image.svg" alt=""></a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
                <ul class="tools">
                    <li class="round"><img  src="/img/image(1).svg" alt=""></li>
                    <li class="round"><img  src="/img/image(3).svg" alt=""></li>
                </ul>
            </div>
        </div>
        <div class="container-lg">
            <div class="row hero-section">
                <ul class="social">
                    <li class="round"><a href="#"><img src="/img/image(4).svg" alt=""></a></li>
                    <li class="round"><a href="#"><img src="/img/image(5).svg" alt=""></a></li>
                    <li class="round"><a href="#"><img src="/img/image(6).svg" alt=""></a></li>
                    <li class="round"><a href="#"><img src="/img/image(7).svg" alt=""></a></li>
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

<style lang="scss">
.section-header{
    background-image:url(/img/banner1.png);
    background-size: cover;
    height: 900px;
}
.container{
    width: 80%;
    margin: 0 auto;
}
.container-lg{
    width: 90%;
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
    }

}
.social{
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
    top:245px;
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