<template>
  <HelloWorld :user="user"/>
  
    <div
    v-if="user.age < 15"
    >
     mon age 
    </div
    
    v-else
    >
     else

    <div>


    </div>

  <input type="text" v-model="user.name" v-on:input="display">
  <input type="text" v-model="user.age">
  </template>
  
  <script setup>
  import HelloWorld from '@/components/HelloWorld.vue';
  import { reactive } from "vue";
  const user = reactive ({
   name: 'NordCoders',
   age: 30,
  });
  
  const display = () => {
    console.log(user.name ,user.age)
  }
   
  display()
  
  </script>
  
  <style>
  
  </style>
  