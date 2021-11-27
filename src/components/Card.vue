<template>
  <div >
    <img :src="image" :alt="title" />
    <h3>{{title}}</h3>     
  </div>
</template>

<script>
export default {
name:'Card',
props:{
    image: String,
    price: String,
    title:String,
    type:String,
},
}
</script>

<style scoped lang="scss">
div{
  text-align:center;
}
h3{
    color:white;
}
</style>