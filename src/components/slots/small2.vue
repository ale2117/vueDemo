<template>
  <div>
    {{ msg }}
    <button @click="changeSmall2">changeSmall2</button>
  </div>
</template>
<script>
export default {
  name:"small2",
  data(){
    return{
      msg:"small2"
    }
  },
  methods:{
    changeSmall2(){
      this.msg = "changedSmall2"
    }
  }
}
</script>
<style>

</style>