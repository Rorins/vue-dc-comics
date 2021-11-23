<template>
  <footer>
      <section><ul>
          <li v-for="(link,index) in navLink" :key="`linkNav-${index}`">
              <a :href="link.url">{{link.text}}</a>
          </li></ul>
          </section>

      <section><ul>
          <li v-for="(link,index) in links" :key="`link-${index}`">
              <a :href="link.url">{{link.text}}</a>
              <li v-for="(link in links.subtitles ,index)" :key="`subLinks-${index}`">
                  <a href="">{{link}}</a>
              </li>
              
          </li>
          </ul></section>

      <section><button>SIGN-UP NOW!</button></section>
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

<style>

</style>