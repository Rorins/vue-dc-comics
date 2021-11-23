<template>
  <!--Header-->
    <header>
      <nav>
        <ul>
          <li v-for="(link,index) in navLink" :key="`link-${index}`">
              <a :href="link.url">{{link.text}}</a>
          </li>

          
        </ul>
      </nav>
    </header>
</template>

<script>
export default {
name: 'Header',
data() {
    return{
        navLink:[
            {
                text:"CHARACTERS",
                url:"/",
                current:true,
            },
            {
                text:"COMICS",
                url:"/",
                current:true,
            },
            {
                text:"MOVIES",
                url:"/",
                current:true,
            },
            {
                text:"TV",
                url:"/",
                current:true,
            },
            {
                text:"GAMES",
                url:"/",
                current:true,
            },
            {
                text:"COLLECTIBLES",
                url:"/",
                current:true,
            },
            {
                text:"VIDEOS",
                url:"/",
                current:true,
            },
            {
                text:"FANS",
                url:"/",
                current:true,
            },
            {
                text:"NEWS",
                url:"/",
                current:true,
            },
            {
                text:"SHOP",
                url:"/",
                current:true,
            },

        ]
    }
}
}
</script>

<style>

</style>