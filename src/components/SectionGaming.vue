<script>

</script>

<template>
    <div class="section">
      <div class="bg-section">
        <div class="container">
            <div class="row">
                <div class="col-6">
                    <h4>Our extreme feature</h4>
                    <h2>The Best Gaming Arena<br>On The World!</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor id totam quidem adipisci
                        veritatis, voluptate laborum architecto blanditiis sequi nobis sunt, eum sapiente voluptatem
                        molestiae mollitia neque labore ducimus enim.</p>
                   
                   

                </div>
                <div class="col-6">
                   <div class="box">
                        <div class="card">
                            <div class="icon-box">
                                <img src="/img/feature1.png" alt="">
                            </div>
                            <h3>Live Streaming</h3>
                            <p>Lorem ipsum dolor sit amet consectetur</p>
                    </div>
                        <div class="card">
                            <div class="icon-box">
                                <img src="/img/feature2.png" alt="">
                            </div>
                                <h3>Gaming News</h3>
                               <p>Lorem ipsum dolor sit amet consectetur</p>
                        </div>
                        <div class="card">
                            <div class="icon-box">
                                <img src="/img/feature3.png" alt="">
                            </div>
                            <h3>Great Tournament</h3>
                            <p>Lorem ipsum dolor sit amet consectetur</p>
                        </div>
                        <div class="card">
                            <div class="icon-box">
                                <img src="/img/feature4.png" alt="">
                            </div>
                            <h3>Awward Ceremony</h3>
                            <p>Lorem ipsum dolor sit amet consectetur</p>
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
    background-image:url(/img/Vector.png);
    background-color: #202046;
    .bg-section{
        background: rgba(25, 25, 53, 0.7);
    }
    
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
    padding:120px 0;
    gap: 0px;
}
.col-6{
    width:50%;
    color:white;
}
.box{
   display:flex;
   justify-content: center;
   align-items:center;
   flex-wrap: wrap;
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
.card{
    width:45%;
    aspect-ratio: 1/1;
    margin: 10px;
    border-radius:20px;
    background-color: #333287 ;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    text-align: center;
    padding:48px 29px;
    &:hover{
        background-color: #05CC7C;
        h3, p{
            color: #202046;
        }
    }
    .icon-box{
        width:100px;
        aspect-ratio:1/1;
        border-radius:200px;
        display:flex;
        justify-content:center;
        align-items: center;
        background-color: #202046;
        padding:17px;
    }
    h3{
        margin-top: 30px;
        margin-bottom:16px;

    }
    p{
        margin: 0;
  
}
}

</style>