<template>

    <div class="AppStackItem">
        <button :class="StackItem"></button>
        <h4>{{StackItemName}}</h4>
    </div>

</template>

<script>
export default{
    props:['StackItem', 'StackItemName']
    
}

</script>

<style>

.AppStackItem button{
    margin: 0rem 1rem;
    border: solid;
    padding: 1.5rem;
    border-width: 2px;
    border-radius: 20px;
    background-size: contain;
}

.AppStackItem{
    text-align: center;
}

.AppStackItem h4{
    font-family: system-ui;
}

</style>