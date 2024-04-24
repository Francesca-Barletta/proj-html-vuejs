<script>
export default {
    props: {
        player: Object
    }

}
</script>


<template>
<div class="card">
    <div class="card-header">
        <img :src="'/img/'+player.url" alt="">
        <div class="new">{{ player.badge }}</div>
    </div>
    <div class="card-body">
        <div class="card-title">
            <h3>{{  player.title }}</h3>
            <h4>{{ player.text }}</h4>
        </div>
        <button class="round"><img :src="'/img/'+player.btn" alt=""></button>
    </div>
</div>
</template>

<style lang="scss" scoped>
.card{
    cursor:pointer;
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