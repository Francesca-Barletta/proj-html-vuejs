<script>

</script>
<template>
    <div class="section">
        <div class="bg-overlay">
            <div class="container">
                <div class="box-header">
                    <div class="title">
                        <div>
                            <h4>Gamer Shop</h4>
                            <h2>Explore Our Shop</h2>
                        </div>
                        <ul class="flex">
                            <li>
                                <button class="white"><img src="/img/image(11).svg" alt=""></button>
                            </li>
                            <li>
                                <button class="green"><img src="/img/image(12).svg" alt=""></button>
                            </li>
                        </ul>

                    </div>
                </div>
                <div class="box-card">
                    <!-- card1 -->
                    <div class="card">
                        <div class="card-header">
                            <img src="/img/s1.png" alt="">

                        </div>
                        <div class="card-body">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <h3>Asus Rog Strix A53</h3>
                            <span class="discount">$960.00</span>
                            <span class="price">$999.00</span>
                        </div>
                    </div>
                    <!-- card2 -->
                    <div class="card">
                        <div class="card-header">
                            <img src="/img/s2.png" alt="">
                        </div>
                        <div class="card-body">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <h3>Asus Rog Strix A53</h3>
                            <span class="discount">$960.00</span>
                            <span class="price">$999.00</span>
                        </div>
                    </div>
                    <!-- card3 -->
                    <div class="card">
                        <div class="card-header">
                            <img src="/img/s3.png" alt="">
                        </div>
                        <div class="card-body">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <h3>Asus Rog Strix A53</h3>
                            <span class="discount">$960.00</span>
                            <span class="price">$999.00</span>
                        </div>
                    </div>
                    <!-- card4 -->
                    <div class="card">
                        <div class="card-header">
                            <img src="/img/s4.png" alt="">
                        </div>
                        <div class="card-body">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="green-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <img class="white-star" src="/img/image(20).svg" alt="">
                            <h3>Asus Rog Strix A53</h3>
                            <span class="discount">$960.00</span>
                            <span class="price">$999.00</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.section{
    background-image: url(/img/shop-bg.png);

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
    width:calc(100%/4);
    margin-top:50px;
}
.card-header{
    background-color: #191935;
    border-radius: 20px;
    height: 260px;
    display:flex;
    justify-content: center;
    align-items: center;
    opacity: 1;
}
.card-body{
    color:white;
    height: 85px;
    padding: 15px;
    img{
        width: 18px;
        margin-right: 5px;
    }
    .green-star{
        filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
    }
    .white-star{
        filter:invert(100%);
    }
   
}
.flex{
    display:flex;
    align-items: center;
    margin-bottom: 13px;
    gap: 7px;
}
.title{
    text-align: center;
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
    button{
        cursor: pointer;
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
    .discount{
        color: #05CC7C;
    }
</style>