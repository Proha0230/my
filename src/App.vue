<template>

<TheHeader></TheHeader>
<MyContact></MyContact>
<AppMyWorksList></AppMyWorksList>



</template>

<script>
import TheHeader from './components/TheHeader.vue';
import AppMyWorksList from './components/AppMyWorksList.vue';
import MyContact from './components/MyContact.vue';
export default{
  components:{TheHeader, AppMyWorksList, MyContact}
}

</script>
