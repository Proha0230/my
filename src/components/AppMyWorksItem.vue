<template>
<div class="myWorksItemMain">
    <div class="myWorksItem">
        <div class="myWorksItemImg">
            <img :src=WorksImg>
        </div>
        <div><h3>{{ WorksName }}</h3></div>
        <div class="MyWorksItemh4"><h4>{{ WorksText }}</h4></div>
        <div class="myWorksItemHref"><a :href=hrefWorks>Перейти на сайт</a></div>
    </div>
</div>

</template>

<script>
export default{
    props:['WorksImg', 'WorksName', 'WorksText', 'hrefWorks']

    
}

</script>

<style>

.myWorksItemImg img{
    width: 20rem;
    height: 12rem;
}
.myWorksItem{
    text-align: center;
    border: solid;
    padding: 1rem;
    border-radius: 25px;
    font-family: system-ui;
    margin: 1rem;
    height: 30rem;
}

.MyWorksItemh4{
    height: 12rem;
}

.myWorksItemHref a{
    border: solid;
    border-width: 2px;
    border-radius: 15px;
    width: 10rem;
    background: khaki;
    color: black;
    padding: 0.3rem;
    text-decoration: none;
}

</style>