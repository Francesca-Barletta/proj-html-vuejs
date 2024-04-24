<script>

</script>
<template>
    <div class="section">

        <div class="container">
            <div class="box-header">
                <div class="title">
                    <div>
                        <h4>Latest News</h4>
                        <h2>Stay Updated With Our<br>Latest News Articles</h2>
                    </div>
                    <ul class="flex">
                        <li>
                            <button class="white"><img src="/img/image(11).svg" alt=""></button>
                        </li>
                        <li>
                            <button class="green"><img src="/img/image(8).svg" alt=""></button>
                        </li>
                    </ul>

                </div>
            </div>
            <div class="box-card">
                <!-- card1 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/b1.png" alt="">
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Ninja Warrior Gaming</h3>
                            <div class="card-info">
                                <div class="icons">
                                    <img src="/img/image(13).svg" alt=""><span>By Admin |</span>
                                    <img src="/img/image(21).svg" alt=""><span>Oct 25, 2022</span>
                                </div>
                                <button class="big">read more<img src="/img/image(8).svg" alt=""></button>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- card2 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/b2.png" alt="">
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Ghost Rider Returns</h3>
                            <div class="card-info">
                                <div class="icons">
                                    <img src="/img/image(13).svg" alt=""><span>By Admin |</span>
                                    <img src="/img/image(21).svg" alt=""><span>Oct 25, 2022</span>
                                </div>
                                <button class="big">read more<img src="/img/image(8).svg" alt=""></button>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- card3 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/b3.png" alt="">
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Call of Deauty 4</h3>
                            <div class="card-info">
                                <div class="icons">
                                    <img src="/img/image(13).svg" alt=""><span>By Admin |</span>
                                    <img src="/img/image(21).svg" alt=""><span>Oct 25, 2022</span>
                                </div>
                                <button class="big">read more<img src="/img/image(8).svg" alt=""></button>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- card-4 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/b4.png" alt="">
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Mortal Combat x</h3>
                            <div class="card-info">
                                <div class="icons">
                                    <img src="/img/image(13).svg" alt=""><span>By Admin |</span>
                                    <img src="/img/image(21).svg" alt=""><span>Oct 25, 2022</span>
                                </div>
                                <button class="big">read more<img src="/img/image(8).svg" alt=""></button>
                            </div>
                        </div>
                    </div>
                </div>


            </div>
        </div>
        <div class="container relative">
            <div class="newsletter">
                <div class="col-6">
                    <h2>Our News Letter</h2>
                </div>
                <div class="col-6">
                    <div class="mail">
                        
                        <span><img src="/img/image(14).svg" alt="">Enter your Email</span>
                        
                        <button>Subscribe</button>
                    </div>
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
.col-6{
    width: 50%;
}

.box-header{
    padding-top:100px;
   
}
.box-card{
    display: flex;
    justify-content:space-around;
    align-items:center;
    gap: 20px;
    padding-bottom: 230px;
}
.card{
    width:calc(100%/4);
    margin-top:50px;
    height: 570px;
    background-color: #202046;
    border-radius: 20px;
   .card-header{
    
    img{
        width: 100%;
        border-radius: 20px 20px 0 0;
        height: 100%;
    }
   }
 
}

.card-body{
    padding: 32px;
    height: 226px;
   
}
.flex{
    display:flex;
    align-items: center;
    margin-bottom: 13px;
    gap: 7px;
}
.title{
    display:flex;
    justify-content: space-between;
    align-items: flex-end;
    h4{
        color: #05CC7C;
        font-size: 20px;
        margin-bottom: 20px;
    }
    h2{
      color:white;
      font-size:47px;
    }
}
.card-title{

    h3{
        font-size: 23px;
        color: white;
        margin-bottom: 23px;
        text-align: center;
    }
}
.green {
    border: none;
    height: 40px;
    aspect-ratio: 1/1;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #05CC7C;

    img {
        width: 20px;
        aspect-ratio: 1/1;
        transform: translateX(10%);
        filter: invert(100%);

    }
}
.white{
    border: none;
    height: 40px;
    aspect-ratio: 1/1;
    border-radius: 9999px;
    display:flex;
    align-items: center;
    justify-content: center;
    background-color:white;
    
    img{
            width: 20px;
            aspect-ratio:1/1;
            transform:translateX(10%);
            filter: brightness(0) saturate(100%) invert(11%) sepia(39%) saturate(1791%) hue-rotate(213deg) brightness(94%) contrast(94%);
          
        }
 }
 .round{
        border: none;
        background-color:#05CC7C;
        height: 55px;
        color:#202046;
        font-size:16px;
        font-weight: 700;
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
    .card-info{
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        color: white;
        gap: 30px;
        align-items: center;
    h3{
     font-size: 28px;
    }
    p{
        font-size:15px;
    }
}
.icons{
display:flex;
gap: 10px;

    img {
        width: 16px;
        aspect-ratio: 1/1;
        filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
    }
}

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
    .relative{
        position: relative;
     
    
    .newsletter{
        position: absolute;
        width: 100%;
        background-color: #202046;
        border-radius: 20px;
        height: 184px;
        top: -100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding:50px;
        h2{
            color: white;
            font-size: 28px;
        }
        .mail{
        background-color: #191935;
        border-radius: 50px;
        width: 100%;
        height: 63px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 10px;
        button{
            background-color: #05CC7C;
            color: #191935;
            height: 50px;
            border-radius:40px;
            display:flex;
            justify-content: center;
            align-items: center;
            padding: 18px;
        }
        img {
        width: 16px;
        aspect-ratio: 1/1;
        margin: 0 5px;
        transform: translateY(4px);
        filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
    }
        span{
            color: grey;
            
        }
        
        }
    }
}
</style>