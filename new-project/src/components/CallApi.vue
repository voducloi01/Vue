<template>
    <div>
        <h1> hello</h1>
    </div>
</template>

<script>
import {ref} from 'vue';
import "babel-polyfill" ;
import 'regenerator-runtime/runtime'
export default {
        setup() {
            const todos= ref([]) ;
            const error= ref(null) ;
            console.log(todos , error);

            const getApi =  async () =>{
                const reponse = await fetch("https://jsonplaceholder.typicode.com/todos") ;
                console.log(reponse) ;
            }

            getApi()
        }
    }
</script>

<style>

</style>