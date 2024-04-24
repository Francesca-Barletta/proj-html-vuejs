<script>
import data from '../assets/db.json'
import ShopCard from './ShopCard.vue'
export default {
    components: {
       ShopCard
    },
    data() {
        return {
           
            products: data.products
        }
    }
}
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
                <ul class="box-card">
                   <li class="col-3" v-for="(product, i) in products" :key="i">
                        <ShopCard :product="product"/>
                  </li> 
                </ul>
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
.col-3{
    width:calc(100%/4);
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

</style>