<script>
export default {
    props: {
        team: Object
    }

}
</script>
<template>
    <div class="card">
        <div class="card-header">
            <img class="overlay" :src="'/img/'+team.img" alt="">
            <img class="card-img" :src="'/img/'+team.img" alt="">

        </div>
        <div class="card-body">
            <div class="card-title">
                <h3>{{ team.name }}</h3>
                <div class="card-info">
                    <div class="icons">
                        <div class="icon"><img :src="'/img/'+team.yt" alt=""></div>
                        <div class="icon"><img :src="'/img/'+team.msg" alt=""></div>
                    </div>
                    <h3>{{ team.time }}</h3>
                    <p>{{ team.date }}</p>
                    <button class="big">{{ team.btn }}</button>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card{
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
.card-title{
    margin-top: 50px;
    text-align: center;
    h3{
    font-size: 35px;
    color: white;
    margin-bottom: 19px;
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
    cursor:pointer;
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
        cursor:pointer;
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
        &:hover{
            background-color:#202046;
            color:#05CC7C;
            border: 1px solid #05CC7C;
            }
     
    }
</style>