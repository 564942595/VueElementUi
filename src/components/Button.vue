<template>
    <div>
        1、elementUI
        <br>
     <span class="wrapper">
        <el-button type="success">成功按钮</el-button>
        <el-button type="warning">警告按钮</el-button>
        <el-button type="danger">危险按钮</el-button>
        <el-button type="info">信息按钮</el-button>
      </span>
      <br><br><br>
       2、父组件给子组件传值，并验证：{{msg}}
       <br><br>
       3、插槽
       <br>
        <slot name="name"></slot>
        <slot></slot> 
    </div>
</template>

<script>
    export default {
        data() {
            return {}
        },
        props:{
            msg:{
                type:String,
            }
        }
    }
</script>

<style lang="sass" scoped>

</style>
