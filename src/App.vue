<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<script setup>
import HelloWorld from './components/HelloWorld.vue'

// This starter template is using Vue 3 experimental <script setup> SFCs
// Check out https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md
</script>

<style>
.card {
  width: 300px;
  height: 400px;
  margin: 30px auto;
  border-radius: 10px;
  box-shadow: 2px 2px 8px #ccc;
  background-color: #f9f9f9;
  overflow: scroll;
}

div {
  padding: 10px;
}

.card img {
  display: block;
  margin: 0 auto;
  width: 100px;
  height: 100px;
  border-radius: 50%;
  padding: 18px;

  object-fit: cover;
  transition: all 0.2s ease-in-out;
}

img:hover {
  transform: scale(1.3);
}

body {
  background-color: #80afcd;
  font-family: Arial, Helvetica, sans-serif;
  display: flex;
  justify-content: center;
  padding: 50px;
  align-items: center;
  min-height: 100vh;
  line-height: 1.4;
}

.card h2 {
  margin: 4px;
  font-size: 21px;
  font-weight: bold;
  text-align: center;
}

.card p {
  margin: 20px;
  font-size: 18px;
  text-align: center;
}

.cool-button {
  background-color: blue;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  display: block;
  margin: auto;
  text-decoration: none;
}

.cool-button:hover {
  background-color: red;
  color: black;
  transform: scale(1.1);
  text-decoration: none;
}
#duplicate {
  background-color: pink;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  display: block;
  margin: auto;
  text-decoration: none;
  position: absolute;
  top: 5%;
  left: 51%;
  transform: translate(-50%, -50%);
  font-weight: bold;
}
#duplicate:hover,
#duplicate:focus {
  background-color: white;
  color: pink;
}

#change-color {
  background-color: pink;
  color: white;
  padding: 10px 30px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  display: block;
  margin: auto;
  position: absolute;
  top: 11%;
  left: 51%;
  transform: translate(-50%, -50%);
  font-weight: bold;
}

#change-color:hover,
#change-color:focus {
  background-color: white;
  color: pink;
}

#change-text {
  background-color: pink;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  display: block;
  margin: auto;
  text-decoration: none;
  position: absolute;
  top: 17%;
  left: 51%;
  transform: translate(-50%, -50%);
  font-weight: bold;
}

#change-text:hover,
#change-color:focus {
  background-color: white;
  color: pink;

  text-decoration: none;
}

.delete {
  background-color: pink;
  color: white;
  padding: 10px 20px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  display: block;
  margin: auto;
  text-decoration: none;
  position: absolute;
  top: 23%;
  left: 51%;
  transform: translate(-50%, -50%);
  font-weight: bold;
}

.delete:hover,
.delete:focus {
  background-color: white;
  color: pink;

  text-decoration: none;
}

@media (max-width: 800px) and (min-width: 500px) {
  .card button {
    display: block;
  }
}

@media (max-width: 500px) {
  .card {
    width: 90%;
  }
}


input:checked + label + .description { display:none; }



</style>
