<script>
import SocialMenu from './SocialMenu.vue';
export default {
    components: {
        SocialMenu
    },
    props: {
        member: Object
    }

}
</script>


<template>
<div class="card">
                    <div class="card-header">
                        <img :src="'/img/'+member.url" alt="">
                        <ul class="social">
                            <SocialMenu/>
                        </ul>
                    </div>
                    <div class="card-body">   
                            <h3>{{ member.name }}</h3>
                            <h4>{{ member.rule}}</h4>
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
                .social {
                    display: block;
                    display: flex;
                    gap: 20px;
                    position: absolute;
                    bottom: 5px;
                    left: 50%;
                    transform: translateX(-50%)
                }
    }
}
.card-header{
    position: relative;
img{
    width:100%;
}
.social{
    display:none;
}
}
.card-body{
    text-align: center;
    background-color: #152257;
    color:white;
    height: 85px;
    padding: 15px;
   
}
</style>
