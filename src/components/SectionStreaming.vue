<script>

</script>

<template>
    <div class="section">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <div class="box">
                        <div class="play">
                            <button class="round"><img src="/img/image(9).svg" alt=""></button>
                            <h4>Call Of Duty</h4>
                        </div>
                        <img src="/img/v-1.png" alt="">
                    </div>

                </div>
                <div class="col-6">
                    <div class="box-header">
                        <div class="title">
                            <div>
                                <h4>Live Streaming</h4>
                                <h2>Check Out Our Live Streming</h2>
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
                        <div class="card">
                            <div class="card-header">
                                <img src="/img/v-small1.png" alt="">
                            </div>
                            <div class="card-body">
                                <h4>Call Of Duty</h4>
                                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="card">
                            <div class="card-header">
                                <img src="/img/v-small2.png" alt="">
                            </div>
                            <div class="card-body">
                                <h4>Assasin Creed</h4>
                                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
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
   
    background-image:url(/img/v-bg.png);
    background-size: cover;
    
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
    gap: 35px;
}
.col-6{
    width:50%;
    color:white;
}
.box{
 border-radius: 22px;
 position:relative;
 .play{
    position:absolute;
    top:40%;
    left:50%;
    transform: translate(-50%);
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    gap: 3px;
    h4{
        color:white;
    }
 }
 
}
.title{
    display:flex;
    justify-content: space-between;
    align-items: flex-end;
    h4{
        color:#05CC7C
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
          
        }
 }
 .round{
    border: none;
    height: 55px;
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
.box-card{
    display: flex;
    justify-content: space-between;
}

h4{
    font-size: 16px;
    margin-top: 20px;
}
h2{
    font-size: 48px;
    margin-top: 0px;
    margin-bottom: 35px;
}
p{
    margin-top: 12px;
    font-size: 13px;
}

.card{
    width: 50%;
    padding: 5px;
}

</style>