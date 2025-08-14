<template>
    <h3>列表渲染</h3>
    <p v-for="(item,index) in names">{{ item }} - {{ index }}</p>
</template>
<script>
export default{
    data(){
        return {
            names:["百战程序员", "尚学堂", "IT"],
        }
    }
}
</script>