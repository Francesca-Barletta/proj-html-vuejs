<script>
import data from '../assets/db.json'
import BattleCard from './BattleCard.vue'
export default{
    components: {
       BattleCard
    },
    data() {
        return {
           
            teams: data.battleTeams

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
                            <h4>Upcoming Match</h4>
                            <h2>Keep Eyes & Manage<br> upcoming Battle</h2>
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

                    <li class="col-4" v-for="(team, i) in teams" :key="i">
                        <BattleCard :team="team" />
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.section{
    background-color: #202046;
    background-image: url(/img/v-bg.png);
    background-size: cover;
   
    .bg-overlay{
        background: rgba(25, 25, 53, 0.7);
    }
    
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
    .col-4{
        width:calc(100%/3);
    }

</style>