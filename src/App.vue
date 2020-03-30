<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>Hello from Vue, {{ name }}!</h1>
    <div class="container">
      <div class="col">
        <div class="field">
          <label for="input-name-1">Ваше имя #1</label>
          <input id="input-name-1" type="text" v-model="name">
        </div>
      </div>
      <div class="col">
        <div class="field">
          <label for="input-name-2">Ваше имя #2</label>
          <input id="input-name-2" type="text" v-model="name">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: () => ({
    name: 'world',
  }),
}
</script>

<style>
body {
  margin: 0;
  background: #f8f9fa;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
}

.container {
  display: flex;
}

.col {
  width: 50%;
  padding-left: 0.25rem;
  padding-right: 0.25rem;
}

.field {
  display: flex;
  flex-direction: column;
}

input {
  border-radius: 4px;
  border: 1px solid #eee;
  padding: 0.5rem 0.75rem;
  outline: none;
}

input:focus {
  border-color: #4CAF50;
  box-shadow: 0 0 8px #4CAF50;
}
</style>
