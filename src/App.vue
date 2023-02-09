<template>
  <div>
    <h1>{{ count }}</h1>
    <div class="btn">
    <button @click="count--">-</button>
    <button @click="count = 0">0</button>
    <button @click="count++">+</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
       count: 26 
       }
  },
};
</script>

<style>
*{
  font-family: 'Roboto', sans-serif;
  font-size: 1.5rem;
  /* color: #333; */
}

body{
  background-image: url('./assets/bg-img.jpeg');
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: center;
}

h1 {
  font-size: 5rem;
  font-weight: 700;
  margin: 0;
  padding: 0;
  color: #000;
}

.btn{
  display: flex;
  justify-content: center;
  align-items: center;
  background: #bbbaba;
  border-radius: 2rem;
  width: 25%;
  margin: 2rem  auto;
}

button {
  background: hsl(0, 1%, 73%);
  border: none;
  border-radius: 2rem;
  padding: 0.5rem 1rem;
  margin: 0.5rem;
  outline: none;
  cursor: pointer;
  color: #402d2d;
  transition: .2s ease-in-out;
  box-shadow: -6px -6px 14px rgba(187, 186, 186, .7),
              -6px -6px 10px rgba(255, 255, 255, .5),
              6px 6px 8px rgba(255, 255, 255, .075),
              6px 6px 10px rgba(0, 0, 0, .15);
}
button:hover {
  box-shadow: -2px -2px 6px rgba(187, 186, 186, .6),
              -2px -2px 4px rgba(255, 255, 255, .4),
              2px 2px 2px rgba(255, 255, 255, .05),
              2px 2px 4px rgba(0, 0, 0, .1);
}
button:active {
  box-shadow: inset -2px -2px 6px rgba(187, 186, 186, .7),
              inset -2px -2px 4px rgba(255, 255, 255, .5),
              inset 2px 2px 2px rgba(255, 255, 255, .075),
              inset 2px 2px 4px rgba(0, 0, 0, .15);
}

#app {
  text-align: center;
  padding: 2rem;
  height: 100vh;
  margin-top: 15%;
}
</style>