<template>
  <!--Second section-->
  <section >
      <div class="container">
      <ul>
          <li v-for="(link,index) in navLink" :key="`linkNav-${index}`">
              <a :href="link.url"><img :src="require(`@/assets/buy-comics-${link.src}.png`)" alt="">{{link.text}}</a>
          </li></ul>
      </div>
  </section>
</template>

<script>
export default {
name:'sectionTwo',
data(){
    return{
        navLink:[
            {
                text:"DIGITAL COMICS",
                url:"/",
                current:true,
                src:"digital-comics",
            },
            {
                text:"DC MERCHANDISE",
                url:"/",
                current:true,
                src:"merchandise",
            },
            {
                text:"SUBSCRIPTION",
                url:"/",
                current:true,
                src:"subscriptions",
            },
            {
                text:"COMIC SHOP LOCATOR",
                url:"/",
                current:true,
                src:"shop-locator",
            },
            {
                text:"DC POWER VISA",
                url:"/",
                current:true,
                src:"digital-comics",
            },
            
        ],
    }
}
}
</script>

<style scoped lang="scss">
section{
    background-color:#0282f9;
    padding:40px 0;
}
ul{
    display:flex;
    list-style-type:none;
}
   li{
       padding:10px;
   }
   a{
       color:white;
       text-decoration:none;
   }
   img{
       width:80px;
   }
</style>