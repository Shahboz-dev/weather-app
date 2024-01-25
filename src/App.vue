
<template>
    <Header/>
    <HeaderContent/>
    <Skills/>
    <Portfolio/> 
    <Footer/>
</template>


<script>
  import Header from "../src/components/Header.vue";
  import HeaderContent from "../src/components/HeaderContent.vue";
  import Skills from "../src/components/Skills.vue"
  import About from "../src/components/About.vue"
  import Portfolio from "../src/components/Portfolio.vue"
  import Footer from "../src/components/Footer.vue"
  import Project from "../src/components/Project.vue"
  export default {
    data(){
      return {}
 }, 
 components:{
  Header,HeaderContent,Skills,About,Portfolio,Footer,Project
 },
 }
</script>


<style scoped>

</style>
