<template>
    <h3>事件传参</h3>
    <p @click="getName(item,$event)" v-for="(item,index) of names" :key="index">
        {{ item }}
    </p>
</template>

<script>

export default{
    data(){
        return{
            names:["iwen","ime","frank"]
        }
    },
    methods:{
        getName(name,event){
            console.log(name);
            console.log(event);
        }
    }
}

</script>