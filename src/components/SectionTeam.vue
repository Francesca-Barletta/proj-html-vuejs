<script>

</script>
<template>
    <div class="section">
        <div class="container">
            <div class="box-header">
                <div class="title">
                    <div>
                        <h4>Team Members</h4>
                        <h2>Our Experts Team<br> Members</h2>
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
                        <img src="/img/team1.png" alt="">
                        
                    </div>
                    <div class="card-body">   
                            <h3>Cristiano Messi</h3>
                            <h4>CEO/Founder</h4>
                    </div>
                </div>
<!-- card2 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/team2.png" alt="">
                    </div>
                    <div class="card-body">
                            <h3>Sergio Naymer</h3>
                            <h4>Programmer</h4>
                    </div>
                </div>
<!-- card3 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/team3.png" alt="">
                    </div>
                    <div class="card-body">
                            <h3>Antonel Roccuzzo</h3>
                            <h4>Project Manager</h4>
                    </div>
                </div>
<!-- card4 -->
                <div class="card">
                    <div class="card-header">
                        <img src="/img/team4.png" alt="">
                    </div>
                    <div class="card-body">
                            <h3>Lionel Ramos</h3>
                            <h4>Game Designer</h4>
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
    }
}
.card-header{
    position: relative;
img{
    width:100%;
}
}
.card-body{
    text-align: center;
    background-color: #152257;
    color:white;
    height: 85px;
    padding: 15px;
   
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
</style>