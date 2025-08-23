<template>
  <!-- <IfDemo />
  <ListDemo /> -->
  <EventDemo1 />
  <EventDemo2 />
  <EventDemo3 />
  <!-- <div v-bind:class="dynamiccla" v-bind:id="dynamicid">测试</div>
  <button :disabled=isornot>Button</button>
  <div v-bind="objectofattrs"> Test</div> -->
</template>

<script>
import IfDemo from './components/IfDemo.vue'
import ListDemo from './components/ListDemo.vue'
import EventDemo1 from './components/EventDemo1.vue'
import EventDemo2 from './components/EventDemo2.vue'
import EventDemo3 from './components/EventDemo3.vue'

export default{
  components:{
    IfDemo,
    ListDemo,
    EventDemo1,
    EventDemo2,
    EventDemo3,
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
