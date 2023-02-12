<template>
  <h1>{{ msg }}</h1>

<!-- My custom code -->
<div class="card">

<img src="https://i.pinimg.com/564x/c4/81/c0/c481c067ad2e11fab13ffe39bc0fd975.jpg" alt="Card Image">

<h2>Welcome</h2>

<p>I was tasked with making a card for this class. I decided to keep it simple and nice. I also decided to add my handsome face to it. </p>


  <button class="cool-button">DETAILS</button>

</div>

<button id="duplicate">DUPLICATION MACHINE</button>
<button id="change-color">COLOR CHANGING MACHINE</button>
<button id="change-text">TEXT CHANGING MACHINE</button>
<button class="delete">DELETING MACHINE</button>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<script>

export default {
  methods: {
    hoover() {
      document.querySelectorAll(".card").forEach((item) => {
        if(!item.classList.contains("hoverCard")){
          item.classList.add("hoverCard");
          console.log(item);
        }
        else{
          item.classList.remove("hoverCard");
          console.log(item);
        }
      });
    },
    
    duplicate() {
      const cloneCard = document.querySelector(".card").cloneNode(true);
      document.body.appendChild(cloneCard);
      console.log(cloneCard);    
    },

    background() {
      document.querySelectorAll(".card").forEach((item) => {
        if(!item.classList.contains("basic")){
          item.classList.add("basic");
          console.log(item);
        }
        else{
          item.classList.remove("basic");
          console.log(item);
        }
      });
    },

    heading() {
      document.querySelectorAll(".title").forEach((item) => {   
        if(item.innerHTML=="something else"){
          item.innerHTML="Chad of Cyber IST";
        }
        else{
          item.innerHTML="something else";
        }
      });
    },

    //Kinda borked rn
    deleter(){
      document.querySelector(".card:last-child").remove();
      console.log(card);
    }
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
