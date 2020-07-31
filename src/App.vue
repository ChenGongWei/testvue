<template>
  <div id="app">
    <Layout />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
import Layout from "./pages/Layout";

export default {
  name: "App",
  components: {
    Layout,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
/* #app { */
/* min-width: 700px; */
/* height: 500px; */
/* } */
</style>
