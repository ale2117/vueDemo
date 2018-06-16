<template>
  <div>
    big
    <button @click="changeView">change</button>
    <keep-alive>
      <component :is="tempView"></component>
    </keep-alive>

  </div>
</template>
<script>
import Small1 from './small1'
import Small2 from './small2'

export default {
  name:"big",
  data(){
    return{
      tempView:"Small1",
      flag: true
    }
  },
  components:{
    Small1,
    Small2
  },
  methods:{
    changeView(){
      if (this.flag) {
        this.tempView = "Small2",
        this.flag = false;
      } else {
        this.tempView = "Small1",
        this.flag = true;
      }
    }
  }
}
</script>
<style>

</style>
