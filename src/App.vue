<template>
  <div id="app">
    <!--HEADER-->
    <Header />

    <!--HERO-->
    <Hero />

    <!--MAIN-->
    <main>
      <sectionOne />
      <sectionTwo />
    </main>

    <!--FOOTER-->
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'
import sectionTwo from '@/components/sectionTwo.vue'
import sectionOne from '@/components/sectionOne.vue'
import Hero from '@/components/Hero.vue'

export default {
  name: 'App',
  components: {
  Header,
  Footer,
  sectionOne,
  sectionTwo,
  Hero,
  }
}
</script>

<style lang="scss">
@import '@/styles/default';
@import '@/styles/utilities';
</style>
