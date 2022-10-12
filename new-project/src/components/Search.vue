<template>
    <div id='account-info'>

        <input type="text" v-model="searchText" />       
         <ul>
            <li v-for="(custom , index) in carFillter" :key="index">
                {{custom}}
            </li>
        </ul>  

        </div>
   </template>
    
   <script>
import { reactive, ref ,computed , watch} from 'vue';
   export default {
    props :['data'],
     setup(props){

      const car = props.data ; 
    
        const so = ref(0) ; 
        const searchText = ref("") ;
        const message = ref("") ;
        const carFillter = computed(()=> car.filter((e) => e.includes(searchText.value) ))
        watch(searchText , (newValue , oldValue) =>{
            console.log(newValue , oldValue);
          }) ;          
          return {searchText , carFillter , message , so}        
      }
   }
   </script>
   