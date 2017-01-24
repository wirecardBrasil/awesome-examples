<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h2> Awesome Mask </h2>
    <p>The awesome-mask runs with Vue.js and uses the vanilla-masker to make your form awesome with masks.</p>
    <h3>Installation</h3>
    <code>
        npm i --save awesome-mask
    </code>
    <h3>Contribute</h3>
    <a href="https://github.com/moip/awesome-mask"> GitHub </a>
    <div class="mdl-textfield mdl-js-textfield">
      <input v-mask="'AAA-9999'" class="mdl-textfield__input" type="text" id="sample1">
      <label class="mdl-textfield__label" for="sample1">Car Plate</label>
    </div>
    <code>
        &lt; input type="text" v-mask="'AAA-9999'" &gt;
    </code>
    <div class="mdl-textfield mdl-js-textfield">
      <input v-mask="'999.999.999-99'" class="mdl-textfield__input" type="text" id="sample2">
      <label class="mdl-textfield__label" for="sample2">CPF</label>
    </div>
    <code>
        &lt; input type="text" v-mask="'999.999.999-99'" &gt;
    </code>

    <div class="mdl-textfield mdl-js-textfield">
      <input v-mask="'99/99/9999'" class="mdl-textfield__input" type="text" id="sample3">
      <label class="mdl-textfield__label" for="sample3">Date</label>
    </div>
    <code>
        &lt; input type="text" v-mask="'99/99/9999'" &gt;
    </code>
  </div>
</template>

<script>
import Hello from './components/Hello'
import AwesomeMask from 'awesome-mask'

export default {
  name: 'app',
  components: {
    Hello
  },
  directives: {
    'mask': AwesomeMask
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
  margin: 60px 0;
}
.mdl-textfield{
  display: block !important;
  margin: 0 auto !important;;
}
code {
  display: inline-block;
  white-space: pre-wrap;
  text-align: left;
  margin: 0 auto;
  background-color: #f2f2f2;
  padding-right: 3em;
  border-radius: 2px;
}
</style>
