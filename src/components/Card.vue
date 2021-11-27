<template>
  <div>
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
  width: 190px;
  padding:5px;
}
img{
  width: 100%;
  object-fit: cover;
}
h3{
    color:white;
}
</style>