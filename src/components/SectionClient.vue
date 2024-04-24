<script>

</script>
<template>
    <div class="section">
        <div class="container">
            <div class="box-header">
                <div class="title">
                        <h4>Testimonials</h4>
                        <h2>What Our Client Say</h2>
                </div>
            </div>
            <div class="box-card">
                <button class="violet"><img src="/img/image(11).svg" alt=""></button>
                <button class="green"><img src="/img/image(8).svg" alt=""></button>
 <!-- card1 -->
                <div class="card">
                   <img src="/img/test1.png" alt="">
                </div>
<!-- card2 -->
                <div class="card">
                    <img src="/img/test2.png" alt="">
                </div>
<!-- card3 -->
                <div class="card">
                    <img src="/img/test3.png" alt="">
                </div>
<!-- card4 -->
                <div class="card">
                    <img src="/img/test4.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.section{
    background-color: #202046;
    background-image: url(/img/test-grouptwo.png);
    background-position: center;
    background-size: cover;
}
.container{
    width:80%;
    margin: 0 auto;
    padding-bottom:100px;
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
    position: relative;
    button{
        cursor:pointer;
    }
}
.card{
    width:calc(100%/4);
    height: 400px;
    margin-top:50px;
    img{
        object-fit: cover;
        height: 120%;
    }
}

.flex{
    display:flex;
    align-items: center;
    margin-bottom: 13px;
    gap: 7px;
}
.title{
  width: 50%;
  text-align: center;
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
.green {
    border: none;
    height: 40px;
    aspect-ratio: 1/1;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #05CC7C;
    position: absolute;
    top: 50%;
    right: 130px;

    img {
        width: 20px;
        aspect-ratio: 1/1;
        transform: translateX(10%);
        filter: invert(100%);

    }
}
.violet {
    border: none;
    height: 40px;
    aspect-ratio: 1/1;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #323288;
    position: absolute;
    top: 50%;
    left: 130px;

    img {
        width: 20px;
        aspect-ratio: 1/1;
        transform: translateX(10%);
        filter: invert(100%);

    }
}

</style>