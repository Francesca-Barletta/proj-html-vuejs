<script>
import data from '../assets/db.json'
import TeamCard from './TeamCard.vue'
export default{
    components: {
       TeamCard
    },
    data() {
        return {
           
            team: data.jobTeam
        }
    }
}
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
            <ul class="box-card">
                <li class="col-3" v-for="(member, i) in team" :key="i">
                    <TeamCard :member="member"/>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.section{
    background-color: #191935;
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