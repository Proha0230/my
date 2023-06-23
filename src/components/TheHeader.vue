<template>
    <div class="MainHeader">
    <div  class="Headerh">      
            <h2 >Ivan Furashov Frontend Dev</h2>  
    </div>
        <div>
            <AppStackList></AppStackList>
        </div>
    </div>

</template>

<script>
import AppStackList from './AppStackList.vue';

export default{
    components:{AppStackList}

}

</script>

<style>

.MainHeader{
    border: solid;
    border-radius: 25px;
    padding: 1rem;
}

.Headerh{
    display: block;
    font-family: system-ui;
    text-align: center;
}



</style>