<template>
  <div>
    <div>
      <button @click="changeArr">click me</button>
      <button @click="changeArr2">click me2</button>
    </div>
    <hr>
    <div v-for="item of arr">
      {{item}}
    </div>
    <hr>
    <div>
      {{obj.a}}
      {{obj.b}}
    </div>
  </div>
</template>


<script>

export default {
  data(){
    return {
      arr:[1,2,3],
      obj:{
        a:1
      }
    }
  },

  mounted(){

  },

  methods:{
    changeArr(){

      // this.arr.push(5)
      this.arr.length = 2
      console.log(this.arr)  // [1,2]
    },

    changeArr2(){
      this.arr.push(6)  // [1,2,6]
    }
  }
}


</script>