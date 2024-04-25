<script>
import data from '../assets/db.json'
import GamingCard from './GamingCard.vue'
export default{
    components: {
       GamingCard
    },
    data() {
        return {
           
            cards: data.gamingCards
        }
    }
}
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
                   <ul class="box">
                        <li v-for="(card, i) in cards" :key="i">
                            <GamingCard :card="card"/>
                        </li>

                    </ul>
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
    background-size: cover;
    .bg-section{
        background: rgba(25, 25, 53, 0.7);
    }
    
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
   li{
    width: 45%;
   }
}

h4{
    color:#05CC7C;
    font-size:25px;
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
    font-size: 20px;
    line-height: 32px;
}

</style>