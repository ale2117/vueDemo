<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <p>
      {{p}}
    </p>
    <h3 v-bind:class="initColor">v-bind 颜色红</h3>
    <h3 v-html="vvv">v-html 颜色红</h3>
    <h3 v-text="vvv">v-text 颜色红</h3>
    <div v-if="isShow">isShow 为true 显示</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcomesssssssssssss to Your Vue.js App',
      p:'this is padding',
      initColor:'red',
      vvv:'<p>vvv</p>',
      isShow:true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
.red{
  color:red
}
</style>
