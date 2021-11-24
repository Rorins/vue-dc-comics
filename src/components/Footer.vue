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
          <img src="../assets/footer-facebook.png" alt=""><img src="" alt=""><img src="" alt=""><img src="" alt=""></div>
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
          links:[
            {
                text:"DC COMICS",
                url:"/",
                current:true,
                maintitle:true,
                subtitles:[
                    "Character","Comics","Movies"
                ]
            },
            {
                text:"DC",
                url:"/",
                current:true,
                maintitle:true,
                subtitles:[
                    "Character","Comics","Movies"
                ]
            },
            {
                text:"SITES",
                url:"/",
                current:true,
                maintitle:true,
                subtitles:[
                    "Character","Comics","Movies"
                ]
            },
            {
                text:"SHOP",
                url:"/",
                current:true,
                maintitle:true,
                subtitles:[
                    "Character","Comics","Movies"
                ]
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
    .social > h3{
        color:#037df0;
        margin-right: 10px;
    }
</style>