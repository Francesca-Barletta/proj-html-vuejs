
<script>
export default {
    props: {
        card: Object
    }

}
</script>

<template>
    <div class="card">
        <div class="icon-box">
            <img :src="'/img/'+card.url" alt="">
        </div>
        <h3>{{ card.title}}</h3>
        <p>{{ card.text }}</p>
    
    </div>    
</template>


<style lang="scss" scoped>

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
        margin-bottom:5px;
        font-size:25px
    }
    p{
        margin: 0;
        font-size:20px
  
}
.card{
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
}

</style>