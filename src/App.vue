<template>
  <div id="app">
    <HeaderComp @changeContent="changeContent" />
    <ContentComp :componentType="componentType" />
    <FooterComp @changeContent="changeContent" />

  </div>
</template>

<script>
import ContentComp from './components/ContentComp.vue'
import HeaderComp from './components/HeaderComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    ContentComp,
    HeaderComp,
    FooterComp
  },
  data () {
    return {
      componentType: 'MainComp'
    }
  },
  methods: {
    changeContent (componentType) {
      this.componentType = componentType
    }
  }
}

</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
