<template>
    <h3>条件渲染</h3>
    <div v-if=flag>你能看见我吗</div>
    <div v-else>那你还是看看我吧</div>
</template>
<!-- v-show也是可以的 -->
<!-- v-if有较高的切换开销,v-show有较高的初始开销 -->
<script>
export default{
    data(){
        return{
            flag:false
        }
    }
}
</script>