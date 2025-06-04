<script setup lang="ts">
  import { ref } from 'vue'
// import HelloWorld from './components/HelloWorld.vue'
// import TheWelcome from './components/TheWelcome.vue'

  const isCalculated = ref(false)

  function calculate(){
    isCalculated.value = true
  }

  function reset(){
    isCalculated.value = false
  }

</script>

<template>
  <div class="page-wrapper dev-border"> 
    <div class="content-wrapper dev-border">
      <div class="info-area dev-border">      

      </div>
      <div class="main-area dev-border">
        XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX<br>
        X <br>
        X <br>
        X <br>
        X <br>
        X <br>
        X <br>
        X <br>

        

      </div>
    </div>
    
  </div>
</template>

<style scoped>
  .info-area {
    border-color: green !important;  
    width: 20rem;
    height: 100%;
  }

  .main-area {
    border-color: blue !important;
    /* max-width: 50%;
    min-width: 460px; */
    /* width: fit-content; */
    height: fit-content;    
    /* flex-grow: 1; */
  }

  .content-wrapper {
    border-color: purple !important;  
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    /* justify-content: center; */
    /* transform: translateX(-20rem); */
    max-width: calc(100%-2.5rem);
  }

  .page-wrapper {
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    justify-content: center;    
    gap: 1.25rem;    

    width: 100vw;
    height: 100vh;
    padding: 1.25rem;
  }

  .dev-border {
    border: 1px dashed red;
  }
</style>
