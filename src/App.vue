
<template>
<body>
  <div id="app">
    <router-view />
  </div>
  <footerVue></footerVue>
</body>
</template>

<script>
import footerVue from "@/components/footerVue.vue";
export default {
  components: {
    "footerVue": footerVue,
  },
 data(){
 return{
 }},
 methods: {
}
};

</script>

<style lang="scss">

body {
    border: none !important;
    margin: 0px !important;
    padding: 0 !important;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0;
}


#footer {
  background-color: #ffffff;
  height: 30px;
  line-height: 30px;
  top: 20px;
  bottom:0;
    a {

      font-weight: bold;
      color: #979797;
      text-decoration: none;
    }
}
</style>
