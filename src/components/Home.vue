
<template>
  <div>
    <my_switch v-model="value1"></my_switch>
    <br>
    <button @click="show">查看值</button>
  </div>
</template>
 
<script>
  import my_switch from "../views/About"; //这里引入上一个文件（目录自己定）
 
  export default {
    components: {
      my_switch
    },
    data() {
      return {
        value1: false //组件的初始状态
      }
    },
    methods: {
      show() {
        alert(this.value1);
      }
    }
  }
</script>