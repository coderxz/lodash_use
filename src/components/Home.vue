<template>
<div>
  hello
</div>
</template>

<script>
export default {
  name: "Home",
  data(){
    return{
      obj:{
        name:'kobe',
        age:43,
        love:{
          call:'d'
        },
        fn(){
          console.log(this.name)
        }
      },
      arr:[1,[2],[3,4],[7,6,7]]
    }
  },
  mounted(){
    //shu zu pian ping hua
    console.log(this.$lodash.flatten(this.arr))
    //sheng ke long
    let deepObj = this.$lodash.cloneDeep(this.obj)
    console.log(deepObj,deepObj===this.obj)
  }
}
</script>

<style scoped>

</style>