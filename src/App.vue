<template>
  <div id="app">
    <!--HEADER-->
    <Header />

    <!--MAIN-->
    <main>
      <sectionOne />
    </main>

    <!--FOOTER-->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import sectionOne from '@/components/sectionOne.vue'

export default {
  name: 'App',
  components: {
  Header,
  Footer,
  sectionOne,
  }
}
</script>

<style lang="scss">
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
}

//UTILITIES
.container{
  max-width: 1170px;
  margin:0 auto;
}
</style>
