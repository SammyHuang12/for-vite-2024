<!-- 寫 JS 區塊 -->
<!-- 把元件拆成小區塊,再滙入 -->
<script setup>
import {ref} from'vue';
const num = ref(2);
function clickMe(){
    num.value++
}
// 這裡不需return
// return{
//     num ,clickMe
// }

// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'

</script>

<!-- html 片段 -->
<template>
   <!-- 應用程式生成的位置 -->
   <div id="app">
    {{ num }}
    <button type="button" v-on:click="clickMe">請點我+1</button>
   </div>
  <!-- <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      
      <HelloWorld msg="You did it!" />  
    </div>
  </header>

  <main>
    <TheWelcome />
  </main> -->


</template>

<!-- css 結構 -->
<style scoped>
/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style>
