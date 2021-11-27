<template>
  <footer>
      <!--First section-->
      <section class="first-section">
          <div class="container">
              <div class="comics-shop">
              <ul>
                  <h3>DC COMICS</h3>
                  <li> <a href="">Characters</a></li>
                  <li><a href="">Comics</a></li>
                  <li><a href="">Movies</a></li>
                  <li><a href="">Tv</a></li>
                  <li><a href="">Games</a></li>
                  <li><a href="">Videos</a></li>
                  <li><a href="">News</a></li>
                  </ul>

              <ul>
                  <h3>SHOP</h3>
                  <li><a href="">Shop DC</a></li>
                  <li><a href="">Shop DC Collectibles</a></li>
                  <li><a href="">Movies</a></li>
                  <li><a href="">Tv</a></li>
                  <li><a href="">Games</a></li>
                  <li><a href="">Videos</a></li>
                  <li><a href="">News</a></li>
                  </ul>
             </div>
             <ul>
                  <h3>Terms of Use</h3>
                  <li><a href="">Privacy policy(New)</a></li>
                  <li><a href="">Ad Choices</a></li>
                  <li><a href="">Advertising</a></li>
                  <li><a href="">Job</a></li>
                  <li><a href="">Subscription</a></li>
                  <li><a href="">Talent Workshop</a></li>
                  <li><a href="">CPSC Certificates</a></li>
                  <li><a href="">Ratings</a></li>
                  <li><a href="">Shop help</a></li>
                  <li><a href="">Contact Us</a></li>
                  </ul>
            
            <ul>
                <h3>SITES</h3>
                  <li><a href="">DC</a></li>
                  <li><a href="">MAD Magazine</a></li>
                  <li><a href="">DC Kids</a></li>
                  <li><a href="">DC Universe</a></li>
                  <li><a href="">DC Power Visa</a></li>
                  </ul>
          <div class="logo">
          </div>
        </div>
    
          </section>

      <!--Second section-->
      <section class="second-section">
          <div class="container">
          <button class="sign-up">SIGN-UP NOW!</button>

          <div class="social"><h3>FOLLOW US</h3>
          <ul class="socialLinks">
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
//first section
.first-section{
    background-image: url(../assets/footer-bg.jpg);
}
    .comics-shop{
        display:block;
    }
    ul {list-style-type: none;}
       h3{
           color:white;
       }
       a{
           color:gray;
           text-decoration: none;
       }
.logo{
    display:flex;
    width:800px;
    background-image:url(../assets/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position:right;
}
//second section
.second-section{
    padding:40px 0;
    background-color: #303030;
}
    div{
        display:flex;
        justify-content: space-between;
        }
        .socialLinks{
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