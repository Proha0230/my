<template>
    <div>
        <div class="myWorksListMain">
            <AppMyWorksItem v-for="item in myWorksData" :key="item"
            :WorksImg = item.WorksImg
            :WorksName = item.WorksName
            :WorksText = item.WorksText
            :hrefWorks = item.hrefWorks
            
            
            ></AppMyWorksItem>
        </div>
    </div>

</template>

<script>
import AppMyWorksItem from './AppMyWorksItem.vue';
import { ref } from 'vue';
export default{
    components:{AppMyWorksItem},
    setup(){

    const myWorksData = ref([
        {WorksText: "Моя игра написанная на Vue3 с использованием Composition API / Vuex / Vue Router / Firebase / AXIOS. В игре присутствует Авторизация и Регистрация нового аккаунта, данные отправляются на сервер Firebase. Эта игра - моя гордость" ,
        WorksName: "Vue3 IF_Count", WorksImg: "https://i.ibb.co/yqtWxMS/If-Count.png", hrefWorks: "https://if-count.web.app/"},
        {WorksText: "Мое приложение написанное на Vue3. Это приложение писал в процессе обучения и практики по Vue3. Это моя собственная идея и те формулы что написаны были для расчетов и работы приложения - лично мои. " ,
        WorksName: "Vue3 Invest_calc", WorksImg: "https://i.yapx.ru/VydDr.png", hrefWorks: "https://proha0230.github.io/calc_invest/"},
        {WorksText: "Мое приложение написанное на Vue3. Это приложение писал в процессе обучения и практики по Vue3. Здесь можно создавать новые задачи, менять их статус, удалять их. Все задачи загружаются на сервер Firebase " ,
        WorksName: "Vue3 IT_Freelance", WorksImg: "https://i.yapx.ru/VyfAT.png", hrefWorks: "https://it-my-freelance.web.app/"},
        {WorksText: "сайт написанный на React - 'React Films'. Для его работы используется 'OMDb API' т.к. база фильмов на Английском языке - в поиске нужно вводить фильмы на Английском языке. Примеры: Matrix, Avengers, Iron Man и т.д.",
        WorksName: "React Films", WorksImg: "https://i.ibb.co/d5mqTYt/React-Films.jpg", hrefWorks: "https://proha0230.github.io/Project-React-Films-GH-Pages/" },
        {WorksText: "сайт написанный на React - 'React Shop Fortnite'. Для его работы используется 'Fortnite API' здесь база товаров на Русском языке. Товары можно добавить в корзину, изменять их кол-во, а так же вовсе удалить из корзины.", 
        WorksName: "React Shop Fortnite", WorksImg: "https://i.ibb.co/fGq7qS6/React-Shop-Fortnite.jpg", hrefWorks: "https://proha0230.github.io/Project-React-Shop-Fortnite-GH-Pages/"},
        {WorksText: "проект SPA на React. Это проект с рецептами блюд. База API-TheMealDB на Англ.яз. В проекте используется Роутинг. Есть переход с категорий блюд к блюдам из выбранной категории и к выбранному рецепту блюда. Поиск работает по категориям блюд.",
        WorksName: "React SPA Food", WorksImg: "https://i.ibb.co/mzsT0f4/React-SPA-FOOD.jpg", hrefWorks: "https://proha0230.github.io/React_SPA_Food_Final_GH_Pages/"},
        {WorksText: "приложение написанное на TypeScript - React. Собрано вручную при помощи WebPack. В приложении можно искать пользователей GitHub. Приложение работает через GitHub API. Есть DARK и LIGHT тема для стилизации приложения по клику на иконки Луны или Солнца.",
        WorksName: "TypeScript GitHub Finder", WorksImg: "https://i.ibb.co/rvHjTC3/GH-Finder.jpg", hrefWorks: "https://proha0230.github.io/Project_TS_GH_Searcher_GH_Pages/"},
        {WorksText: "сайт на Native JavaScript. Cобран при помощи Gulp & Webpack. Нажав на кнопку 'РАССЧИТАТЬ СТОИМОСТЬ' откроется калькулятор где клиент вводит параметры и выбирает материал окон, теплый/холодный метод остекления - все данные отправляются формой на сервер.",
        WorksName: "Native JavaScript Ирвас Окна", WorksImg: "https://i.ibb.co/BgMYYgn/image.jpg", hrefWorks: "https://proha0230.github.io/Project_JS_Irvas_Okna/"},
        {WorksText: "сайт на Native JavaScript. Аккордеон, Слайдер, Модальные окна, Плавная анимация прокрутки страницы благодаря hash и requestAnimationFrame, Реализована возможность drag & drop загрузки изображений, Телефонная маска, Валидация полей для ввода имени/email и т.п.",
        WorksName: "Native JavaScript Картины.ART", WorksImg: "https://i.ibb.co/HrkGxSz/ART.jpg", hrefWorks: "https://proha0230.github.io/Project_JS_PICTURES_ART/"}
    ])


    return{myWorksData}
    }

}

</script>

<style>

.myWorksListMain{
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    place-content: center;
}

@media (min-width: 810px) and (max-width: 1204px){

.myWorksListMain{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    place-content: center;
}

.MyWorksItemh4 {
    height: 12rem;
}

.myWorksItem {
    height: 30rem;
}

}

@media (min-width: 701px) and (max-width: 809px){

.myWorksListMain{
    display: grid;
    grid-template-columns: repeat(2, 350px);
    place-content: center;
}

.myWorksItemImg img{
    width: 17rem;
    height: 11rem;
}

.MyWorksItemh4 {
    height: 14rem;
}

.myWorksItem {
    height: 31rem;
}

}

@media (min-width: 600px) and (max-width: 700px){

.myWorksListMain{
    display: grid;
    grid-template-columns: repeat(2, 300px);
    place-content: center;
}

.myWorksItemImg img{
    width: 14rem;
    height: 10rem;
}

.myWorksItem {
    height: 34.5rem;
}

.MyWorksItemh4 {
    height: 17rem;
}
}

@media (min-width: 446px) and (max-width: 599px){

.myWorksListMain{
display: grid;
grid-template-columns: repeat(1, 1fr);
place-content: center;
}

.myWorksItem {
    height: 29rem;
}

.MyWorksItemh4 {
    height: 11rem;
}

}

@media (min-width: 335px) and (max-width: 445px){

.myWorksListMain{
display: grid;
grid-template-columns: repeat(1, 350px);
place-content: center;
}

.myWorksItem {
    height: 32rem;
}

.MyWorksItemh4 {
    height: 14rem;
}

.myWorksItemImg img{
    width: 17rem;
    height: 12rem;
}
}
</style>