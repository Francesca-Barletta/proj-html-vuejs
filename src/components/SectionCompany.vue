<script>

</script>

<template>
    <div class="section">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <div class="box">
                        <div class="box-exp">
                            <img class="shape1" src="/img/shape1.png" alt="">
                            <img class="shape2" src="/img/shape2.png" alt="">
                            <img class="shape-grid" src="/img/exprience-shape.png" alt="">
                            <img class="main-img" src="/img/exprince.jpg" alt="">

                        </div>
                    </div>

                </div>
                <div class="col-6">
                    <div class="title">
                        <h4>12 Year Experience</h4>
                    <h2>We Are The Best Gaming Company</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor id totam quidem adipisci
                        veritatis, voluptate laborum architecto blanditiis sequi nobis sunt, eum sapiente voluptatem
                        molestiae mollitia neque labore ducimus enim.</p>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora, autem.</p>
                    </div>
                    <ul>
                        <li class="flex">
                            <div class="icon"><img src="/img/image(10).svg" alt=""></div> ipsum, dolor sit amet
                            consectetur.
                        </li>
                        <li class="flex">
                            <div class="icon"><img src="/img/image(10).svg" alt=""></div> ipsum, dolor sit amet
                            consectetur adipisicing elit.
                        </li>
                        <li class="flex">
                            <div class="icon"><img src="/img/image(10).svg" alt=""></div> ipsum, dolor sit amet
                            consectetur adipisicing elit.
                        </li>
                        <li class="flex">
                            <div class="icon"><img src="/img/image(10).svg" alt=""></div> ipsum, dolor sit amet
                            consectetur adipisicing elit.
                        </li>
                    </ul>
                    <ul class="buttons">
                        <li><button class="big">Discover more<img src="/img/image(8).svg" alt=""></button></li>
                        <li><button class="round"><img src="/img/image(9).svg" alt=""></button></li>
                    </ul>
                </div>
            </div>
        </div>


    </div>

</template>

<style lang="scss" scoped>
.section{
    background-color: #191935;
}
.container{
    width:80%;
    margin: 0 auto;
}
.flex{
    display:flex;
    align-items: center;
    margin-bottom: 13px;
    gap: 7px;
}
.row{
    display:flex;
    align-items: center;
    justify-content: center;
    padding-top:270px;
    padding-bottom: 100px;
    gap: 70px;
}
.col-6{
    width:50%;
    color:white;
}
.box{
    padding-top: 24px;
    padding-bottom: 45px;
    background-color: #191935;
}
.box-exp{
    width:100%;
    aspect-ratio: 1/1;
    position:relative;
    .shape1 {
            position: absolute;
            top: 0;
            left: 0;
            width: 80%;
        }
    
    .shape2 {
            position: absolute;
            bottom: 0;
            right: 0;
        }
    
    .shape-grid {
            position: absolute;
            top: 33px;
            left: -72px;
            width: 112px;
        }
    
    .main-img {
            position: absolute;
            top: 50px;
            left: 50px;
            width: 85%;
        }
}
.title{
    h4{
        color: #05CC7C;
        font-size: 20px;
        margin-bottom: 20px;
    }
    h2{
      color:white;
      font-size:47px;
    }
    p{
        font-size: 20px;
        line-height: 30px;
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
h4{
    color:#05CC7C;
    font-size:16px;
    margin-bottom: 26px;
}
h2{
    font-size: 48px;
    margin-top: 0px;
    margin-bottom: 40px;
}
p{
    margin:20px 0;
    margin-bottom: 30px;
}
.icon{
    width:26px;
    aspect-ratio: 1/1;
    border: 1px solid #05CC7C;
    border-radius: 100px;
    padding:2px;
    margin-right: 2px;
    display: flex;
    justify-content: center;
    align-items: center;
    img{
        width:14px
    }
}
</style>