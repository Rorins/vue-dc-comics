<template>
  <section class="container">
      <ul>
          <li v-for="(link,index) in navLink" :key="`linkNav-${index}`">
              <a :href="link.url">{{link.text}}</a>
          </li></ul>
  </section>
</template>

<script>
export default {
name:'sectionOne',
data(){
    return{
        navLink:[
            {
                text:"DIGITAL COMICS",
                url:"/",
                current:true,
            },
            {
                text:"DC MERCHANDISE",
                url:"/",
                current:true,
            },
            {
                text:"SUBSCRIPTION",
                url:"/",
                current:true,
            },
            {
                text:"COMIC SHOP LOCATOR",
                url:"/",
                current:true,
            },
            {
                text:"DC POWER VISA",
                url:"/",
                current:true,
            },
            
        ],
    }
}
}
</script>

<style scoped lang="scss">
ul{
    display:flex;
}
</style>