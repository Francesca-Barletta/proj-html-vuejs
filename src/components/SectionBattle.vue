<script>

</script>
<template>
    <div class="section">
        <div class="bg-overlay">
            <div class="container">
                <div class="box-header">
                    <div class="title">
                        <div>
                            <h4>Upcoming Match</h4>
                            <h2>Keep Eyes & Manage<br> upcoming Battle</h2>
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
                            <img class="overlay" src="/img/m1.png" alt="">
                            <img class="card-img" src="/img/m1.png" alt="">

                        </div>
                        <div class="card-body">
                            <div class="card-title">
                                <h3>Ninja Warrior Gaming</h3>
                                <div class="card-info">
                                    <div class="icons">
                                        <div class="icon"><img src="/img/image(13).svg" alt=""></div>
                                        <div class="icon"><img src="/img/image(14).svg" alt=""></div>
                                    </div>
                                    <h3>9.45</h3>
                                    <p>1st November, 2022</p>
                                    <button class="big">View more</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- card2 -->
                    <div class="card">
                        <div class="card-header">
                            <img class="overlay" src="/img/m2.png" alt="">
                            <img class="card-img" src="/img/m2.png" alt="">

                        </div>
                        <div class="card-body">
                            <div class="card-title">
                                <h3>Witch Gaming</h3>
                                <div class="card-info">
                                    <div class="icons">
                                        <div class="icon"><img src="/img/image(13).svg" alt=""></div>
                                        <div class="icon"><img src="/img/image(14).svg" alt=""></div>
                                    </div>
                                    <h3>9.45</h3>
                                    <p>1st November, 2022</p>
                                    <button class="big">View more</button>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- card3 -->
                    <div class="card">
                        <div class="card-header">
                            <img class="overlay" src="/img/m3.png" alt="">
                            <img class="card-img" src="/img/m3.png" alt="">

                        </div>
                        <div class="card-body">
                            <div class="card-title">
                                <h3>SkullG Gaming</h3>
                                <div class="card-info">
                                    <div class="icons">
                                        <div class="icon"><img src="/img/image(13).svg" alt=""></div>
                                        <div class="icon"><img src="/img/image(14).svg" alt=""></div>
                                    </div>
                                    <h3>9.45</h3>
                                    <p>1st November, 2022</p>
                                    <button class="big">View more</button>
                                </div>
                            </div>
                        </div>
                    </div>
                  

                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.section{
    background-color: #202046;
    background-image: url(/img/v-bg.png);
   
    .bg-overlay{
        background: rgba(25, 25, 53, 0.7);
    }
    
}
.container{
    width:80%;
    margin: 0 auto;
}
.box-header{
    padding-top:100px;
   
}
.box-card{
    display: flex;
    justify-content:space-around;
    align-items:center;
    gap: 20px;
    padding-bottom: 100px;
}
.card{
    width:calc(100%/3);
    margin-top:50px;
    height: 725px;
    background-color: #202046;
    border-radius: 20px;
    padding: 28px;
 
}
.card-header{
    background-color: #191935;
    height: 330px;
    border-radius: 20px;
    position: relative;
    .card-img{
        position: absolute;
        top: 12%;
        left: 50%;
        transform: translateX(-50%);
        height: 228px;
    }
    img.overlay{
        opacity: 0.1;
        position: absolute;
        right: 1px;
       height: 300px;
    }
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
    margin-top: 50px;
    text-align: center;
    h3{
    font-size: 35px;
    color: white;
    margin-bottom: 19px;
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
    align-items: center;
    justify-content: center;
    color: white;
    gap: 13px;
    h3{
     font-size: 43px;
     margin:0;
    }
    p{
        font-size:18px;
    }
}
.icons{
    display: flex;
    gap: 12px;
}
.icon {
    border: none;
    height: 40px;
    aspect-ratio: 1/1;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #05CC7C;

    img {
        width: 16px;
        aspect-ratio: 1/1;
        filter: brightness(0) saturate(100%) invert(11%) sepia(39%) saturate(1791%) hue-rotate(213deg) brightness(94%) contrast(94%);
        

    }
}
.big{
        border: none;
        background-color:#05CC7C;
        height: 55px;
        color:#202046;
        font-size:16px;
        font-weight: 700;
        padding: 0 32px;
        border-radius:4px;
        display:flex;
        align-items: center;
        
     
    }
</style>