<template xmlns:v-bind="http://www.w3.org/1999/xhtml">
  <div>
    <img src="./assets/logo.png">
    <router-view/>
    <!--<div id="app-1">
          {{ message }}
    </div>
    &lt;!&ndash; v-for &ndash;&gt;
    <div id="app-2">
          <ul>
            <li v-for = "input in inputs">
              {{input}}
            </li>
          </ul>
    </div>
    <div id="hw" >
        12323323
    </div>-->
    <div class="hw1" >
      12323323
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      message : 'Hello word!',
      inputs:['text','select','radio']
    }
  }
}
</script>

<style>
.app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.hw1{
  height: 100px;
  width: 100px;
  background-color: red;
}
</style>
