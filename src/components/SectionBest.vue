<script>

</script>
<template>
    <div class="section">
        <div class="bg-overlay">
            <div class="container">
            <div class="box-header">
                <div class="title">
                    <div>
                        <h4>Trending Games</h4>
                        <h2>Choose Who Is the best<br> in world!</h2>
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
                        <img src="/img/protfolio1.png" alt="">
                        <div class="new">New</div>
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Assassin's Creed</h3>
                            <h4>Lorem ipsum dolor sit amet.</h4>
                        </div>
                        <button class="round"><img src="/img/image(9).svg" alt=""></button>
                    </div>
                </div>
<!-- card2 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/protfolio2.png" alt="">
                        <div class="new">New</div>
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Call Of Deauty</h3>
                            <h4>Lorem ipsum dolor sit amet.</h4>
                        </div>
                        <button class="round"><img src="/img/image(9).svg" alt=""></button>
                    </div>
                </div>
<!-- card3 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/protfolio3.png" alt="">
                        <div class="new">New</div>
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Tomb Raider</h3>
                            <h4>Lorem ipsum dolor sit amet.</h4>
                        </div>
                        <button class="round"><img src="/img/image(9).svg" alt=""></button>
                    </div>
                </div>
<!-- card4 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/protfolio4.png" alt="">
                        <div class="new">New</div>
                    </div>
                    <div class="card-body">
                        <div class="card-title">
                            <h3>Mortal Combat X</h3>
                            <h4>Lorem ipsum dolor sit amet.</h4>
                        </div>
                        <button class="round"><img src="/img/image(9).svg" alt=""></button>
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
    background-image: url(/img/protfolio-vector.png);
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
    cursor:pointer;
    width:calc(100%/4);
    margin-top:50px;
    &:hover{
        .card-body{
            background-color: #05CC7C;
        }
        .round{
            background-color: #152257;
            img{
                filter: brightness(0) saturate(100%) invert(58%) sepia(52%) saturate(7406%) hue-rotate(125deg) brightness(97%) contrast(101%);
            }
        }
    }
}
.card-header{
    position: relative;
    .new{
            position: absolute;
            display: flex;
            align-items: center;
            justify-content: center;
            top: 0;
            left: 0;
            color: #191935;
            background-color: #05CC7C;
            width: 60px;
            height: 40px;
        }
        img{
            width: 100%;
        }
}
.card-body{
   
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 5px;
    background-color: #152257;
    color: white;
    padding: 24px 15px;

    .card-title{
        h3{
            font-size: 23px;
             margin-bottom: 10px;
        }
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
 .round{
    border: none;
    background-color: #05CC7C;
    height: 55px;
    font-size: 16px;
    aspect-ratio: 1 / 1;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;

        img{
            width: 20px;
            aspect-ratio:1/1;
            transform:translateX(10%);
            filter: brightness(0) saturate(100%) invert(11%) sepia(39%) saturate(1791%) hue-rotate(213deg) brightness(94%) contrast(94%);
        }
    
    }
</style>