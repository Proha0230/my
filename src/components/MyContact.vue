<template>
<div class="mainContact">
        <div>
            <h3>Мои контакты:</h3>
        </div>
        <div class="MyContactPage">
            <h3>Email: Proha0230@yandex.ru</h3>
            <h3>GitHub: Proha0230</h3>
            <h3>Telegram: @Proha0230</h3>
        </div>
        <div>
            <h2>Мои Работы:</h2>
        </div>
</div>

</template>

<script>
export default{

}
</script>

<style>

.mainContact {
    text-align: center;
    font-family: system-ui;
}

.MyContactPage{
    display: inline-flex;
}

.MyContactPage h3{
    margin: 1rem;
}


@media (min-width: 260px) and (max-width: 516px){

.MyContactPage{
    display: inline-block;
}

}

</style>