<template>
  <IfDemo />
  <div v-bind:class="dynamiccla" v-bind:id="dynamicid">测试</div>
  <button :disabled=isornot>Button</button>
  <div v-bind="objectofattrs"> Test</div>
</template>

<script>
import IfDemo from './components/IfDemo.vue'
export default{
  components:{
    IfDemo
  },
  data(){
    return{
      dynamiccla:"active",
      dynamicid:"dynamicid",
      isornot:false,
      objectofattrsP:{
        class:"appclass",
        id:"appid"
      }
    }
  }
}
</script>

<style>

.active{
  color: red;
  font-size: 20px;
}

</style>
