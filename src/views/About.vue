<template>
  <div>
    momo
    <p>{{msg}}</p>
    <input v-model="msg">
    <Child @qqq="fun2" :age="age" />
    <button @click="ageAdd">变大</button>
  </div>
</template>

<script>

import Child from '../components/Child'



export default {
  name:'momo',
  components:{
    Child
  },
  data(){
    return {
      msg:'Hi',
      timer:null,
      age:15
    }
  },

  methods:{
    ageAdd(){
      this.age++
    },

    fun2(data){
      console.log('我是子组件传递过来的')
      console.log(data)
    }
  },

  // beforeCreate(){
  //   console.log('beforeCreate')
  // },
  // created(){
  //   console.log('created')
  // },
  // beforeMount(){
  //   console.log('beforeMount')
  // },
  mounted(){
    // console.log('mounted')
    // this.timer = setInterval(() => {
    //   console.log(111)
    //   console.log(this.timer)
    // }, 1000)
  },

  // updated(){
  //   console.log('updated')
  // },
  // beforeDestroy(){
  //   console.log('beforeDestroy')
  // },
  // destroyed(){
  //   console.log('destroyed')
  //   clearInterval(this.timer)
  // }



}


</script>

<style lang="scss" scoped>

</style>