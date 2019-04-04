<template>
  <div id="app">
     <v-button :msg="msg" >
       <h4>普通插槽</h4>
       <h3 slot='name'>具名插槽，只在有name的slot中显示</h3>
       <h4>普通插槽</h4>
     </v-button>
     <v-animation></v-animation>
  </div>
</template>

<script>
  import Button from './components/Button.vue'
  import Animation from './components/animate.vue'
export default {
  name: 'App',
  data(){
    return {
      msg:"父组件传过来的值"
    }
  },
  components:{
    'v-button':Button,
    'v-animation':Animation
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
