<template>

<div class="AppStackList">
<AppStackItem v-for="item in StackItemData" :key="item"
:StackItemName = item.StackItemName
:StackItem = item.StackItem

></AppStackItem>
</div>

</template>

<script>
import AppStackItem from './AppStackItem.vue';
import { ref } from 'vue';

export default{
    components:{AppStackItem},
    setup(){

    const StackItemData = ref([
        {StackItemName: 'JavaScript', StackItem: 'JS'},
        {StackItemName: 'Vue3', StackItem: 'Vue3'},
        {StackItemName: 'React', StackItem: 'React'},
        {StackItemName: 'Firebase', StackItem: 'Firebase'},
        {StackItemName: 'AXIOS', StackItem: 'AXIOS'},
        {StackItemName: 'HTML', StackItem: 'HTML'},
        {StackItemName: 'CSS', StackItem: 'CSS'},
        {StackItemName: 'webpack', StackItem: 'webpack'}
    ])

        return{StackItemData}
    }
    
}

</script>

<style>

.AppStackList{
    display: grid;
    grid-template-columns: repeat(8, 1fr);
}

.JS{
    background-image: url(../assets/JS.png);
}
.Vue3{
    background-image: url(../assets/logo.png);
}
.React{
    background-image: url(../assets/React.png);
}
.HTML{
    background-image: url(../assets/HTML.png);
}
.CSS{
    background-image: url(../assets/CSS.png);
}
.Firebase{
    background-image: url(../assets/Firebase.png);
}
.AXIOS{
    background-image: url(../assets/AXIOS.png);
}
.webpack{
    background-image: url(../assets/webpack.png);
}

@media (min-width: 380px) and (max-width: 812px){

.AppStackList{
display: grid;
grid-template-columns: repeat(4, 1fr);
}
}

@media (min-width: 315px) and (max-width: 379px){

.AppStackList{
display: grid;
grid-template-columns: repeat(4, 80px);
justify-content: center;
}
}

@media (min-width: 260px) and (max-width: 314px){

.AppStackList{
display: grid;
grid-template-columns: repeat(3, 80px);
justify-content: center;
}
}

</style>