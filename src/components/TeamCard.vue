<script>
export default {
    props: {
        member: Object
    }

}
</script>


<template>
<div class="card">
                    <div class="card-header">
                        <img :src="'/img/'+member.url" alt="">
                        
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
</style>
