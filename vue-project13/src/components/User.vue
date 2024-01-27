<template>
    <div class="card" v-bind:class="{ color: isTrue}">
        <h3>{{ user.name }}</h3>
        <p class="desc">{{ user.description }}</p>
        <p>{{ user.price }}</p>
        <button class="butt" @click="changeColor">В избранное</button>
    </div>
</template>
<script>
export default {
    props: {
        user: Object,
    },
    data(){
        return{
            isTrue: false,
        }
    },
    methods:{
        changeColor(){
            this.isTrue = !this.isTrue
        }
    }
}
</script>
<style>
    .card{
        margin: 16px;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 500px;
        border-radius: 7%;
        background-color: rgb(241, 238, 238);
    }
    .desc{
        margin: 0 20%;
    }
    .butt{
        margin: 0px 10px 10px;
        background-color: orange;
        width: 166px;
        height: 44px;
        border-radius: 7%;
    }
    .color{
        background-color: red;
    }
</style>