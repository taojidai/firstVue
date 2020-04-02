<template>
  <div>
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <div :class="[hw,colorGreen]">
          1232222
    </div>
    <button v-on='{mouseenter:onEnter,mouseleave:onOut}' @keyup.enter="onClick">点我</button>
    <button v-on='{mouseenter:onEnter,mouseleave:onOut}' @click="onClick">点我1</button>
    <input v-model="inputValue" placeholder="请输入">
    <span>{{inputValue}}</span>
    <select v-model="selected">
      <option value="" disabled>请选择</option>
      <option value="A" >A</option>
      <option value="B" >B</option>
      <option value="C" >C</option>
    </select>
    <span>selected:{{selected}}</span>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    data () {
      return {
        msg: 'Welcome to Your Vue.js App',
        hw:'hw',
        colorGreen:'colorGreen',
        inputValue:'',
        selected:''
      }
    },
    methods : {
      onClick : function(){
        console.log("clicked");
        console.log("selected:"+ this.selected);
      },
      onEnter : function(){
        console.log("mouseenter");
      },
      onOut : function(){
        console.log("mouseout");
      },
      onSubmit:function() {
        console.log("submitted");
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1, h2 {
    font-weight: normal;
  }
  .hw{
    height: 100px;
    width: 100px;
    background-color: red;
  }
  .colorGreen{
    background-color: #42b983;
  }
</style>
