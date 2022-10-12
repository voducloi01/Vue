<template>
    <div>
        <input type="text" v-model="name" />
        <h1> {{name}}</h1>
    </div>
</template>

<script>
import {ref} from 'vue'
export default {
    name: 'Vue1Vmodel',
    setup() {
        const name = ref("")
        return { name}
    }
};
</script>

<style>

</style>