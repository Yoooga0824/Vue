<template>  
  <h3>模板语法</h3>
  <p>{{ msg }}</p>
  <p>{{ number + 1 }}</p>
  <p v-html = "rawHtml"></p>
</template>

<script>
export default{
  data(){
    return{
      msg:"Hello Vue3",
      number:10,
      rawHtml:"<a href='https://itbaizhan.com'>百战程序员</a>"
    }
  }
}
</script>

