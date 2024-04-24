<script>
import StarsValue from './StarsValue.vue'
export default {
    components: {
       StarsValue
    },
    props: {
        product: Object
    }

}
</script>

<template>
    <div class="card">
        <div class="card-header">
            <img :src="'/img/'+product.url" alt="">

        </div>
        <div class="card-body">
            <StarsValue />
            <h3>{{ product.name }}</h3>
            <span class="discount">{{ product.discount }}</span>
            <span>{{ product.price }}</span>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.card{
   
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
    h3{
        margin-top: 14px;
        margin-bottom: 10px;
    }
    span{
        margin-right: 3px;
    }
    .discount{
        color: #05CC7C;
    }
}

</style>