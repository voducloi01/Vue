<template>
   <div>
        <div v-show="isComplete">
            <h1 >Vue</h1>
            
        </div>
        <div>
            <button @click='show'>Bấm</button>
        </div>
   </div>
</template>

<script>
import {ref} from 'vue'
export default {
    name: 'Vue1Show',

   setup() {

    let isComplete = ref(true)  ;

    function show () {
      return isComplete.value = !isComplete.value;
    }

    return {isComplete ,  show}
   }
};
</script>

<style >

</style>