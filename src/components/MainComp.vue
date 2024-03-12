<template>
  <component :is="componentType" />
</template>

<script>
import ContentComp from './components/ContentComp.vue'

export default {
  name: 'MainComp',
};
</script>


<style scoped>
    html {
    scroll-behavior: smooth;
    }

    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    }

    a {
    text-decoration: none;
    }

    a:visited {
    color: inherit;
    }

    .center {
    padding-left: calc(50% - 600px);
    padding-right: calc(50% - 600px);
    }

    .container {
    display: flex;
    flex-direction: column;
    align-items: center;
    }


    .header {
    width: 1200px;
    padding: 50px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
    }
    .header__menubar {
    display: flex;
    gap: 50px;
    color: rgb(41, 47, 54);
    font-family: "Jost", sans-serif;
    font-weight: 400;
    font-size: 20px;
    }
</style>