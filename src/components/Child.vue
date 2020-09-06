<template>
  <div>
    <p>my son is {{age}} years old</p>
    <div @click="fun">点我,然后我就向父组件传递数据了</div>
  </div>
</template>


<script>
export default {
  props:{
    age:{
      type:Number,
      default:3
    }
  },
  name:'child',
  data(){
    return {

    }
  },
  methods:{
    fun(){
      this.$emit('qqq',{age:18,name:'zhangsan'})
    }
  }
}


</script>
