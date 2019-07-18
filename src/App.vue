<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Test v-slot="{team}">
      <h2>Hello world! my team is {{team}}</h2>
      <!-- <p slot="paragraph">Hello, I am a paragraph text</p>
      <ul slot="links">
        <li>Hello, I am a list item</li>
        <li>Hello, I am a list item</li>
      </ul> -->
    </Test>
  </div>
</template>

<script>
import Test from './components/Test.vue'

export default {
  name: 'app',
  components: {
    Test
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
