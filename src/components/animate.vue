<template>
    <div>
       <transition  
            enter-active-class="animated flash"
            leave-active-class="animated shake"
        >
         <h2 v-show="show">我是动画内容的文字</h2>
       </transition>
       <button @click='animate()'>动画</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
              show:true,
            }
        },
        props:{
           
        },methods:{
          animate(){
            this.show=!this.show;
          }
        }
    }
</script>

<style lang="sass" scoped>

</style>
