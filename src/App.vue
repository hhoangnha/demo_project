<template>
  <div id="app">
    <!-- <p v-for="a in arr">{{a}}</p> -->
    <p id="demo">{{msg}}</p>
    <demo></demo>
    <button type="button" @click="abc">click</button>
  </div>
</template>

<script>
import demo from './demo'
import $ from 'jquery'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      arr:[1,2,3]
    }
  },
  methods:{
    abc(){
      $("#demo").text("ok")
    }
  },
  components:{
    demo
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

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
