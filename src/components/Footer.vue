<template>
  <footer>
      <!--First section-->
      <section class="first-section">
          <div class="container">
          <ul><li v-for="(link,index) in navLink" :key="`linkNav-${index}`">
              <a :href="link.url">{{link.text}}</a></li></ul>
          </div>
          </section>

      <!--Second section-->
      <section class="second-section">
          <div class="container">
          <button class="sign-up">SIGN-UP NOW!</button>

          <div class="social"><h3>FOLLOW US</h3>
          <ul>
          <li v-for="(icon,index) in social" :key="`socialIcon-${index}`">
              <img :src="require(`@/assets/footer-${icon.src}.png`)" alt="">
          </li>
          </ul>
          </div>

          </div>

          </section>

  </footer>
</template>

<script>
export default {
name: 'Footer',
data() {
    return{
        navLink:[
            {
                text:"DIGITAL COMICS",
                url:"/",
                current:true,
            },
            {
                text:"DC",
                url:"/",
                current:true,
            },
            {
                text:"SITES",
                url:"/",
                current:true,
            },
            {
                text:"SHOP",
                url:"/",
                current:true,
            },
            
        ],
        social:[
            {
                src:'facebook',
            },
            {
                src:'periscope',
            },
            {
               src:'pinterest',
            },
            {
                src:'twitter',
            },
            {
                src:'youtube',
            },
            
        ]
    }
}
}
</script>

<style scoped lang="scss">
.first-section{
    background-image: url(../assets/footer-bg.jpg);
    padding:40px 0;
}
    ul {list-style-type: none;}
       a{
           color:white;
           text-decoration: none;
       }
.second-section{
    padding:40px 0;
    background-color: #303030;
}
    div{
        display:flex;
        justify-content: space-between;
        align-items: center;
        }
    ul{
        display:flex;
    }
    li{
        padding:5px;
    }
    .social > h3{
        color:#037df0;
        margin-right: 10px;
    }
</style>