<template>
<div>
  <!-- data binding using double curly braces-->
    <h1>{{greet}} {{name}}</h1>

  <!-- data binding using v-text directive. Drawback of v-text is it replaces entire html element.-->
    <h1 v-text="channel"></h1>


</div>

</template>

<script>


export default {
  name: 'App',
  //using data() function to initialize properties: think of ot like a constructor for a class
  data()
  {
    return {
      greet:"Hello",
      name:"binding text using double curly braces",
      channel:"binding text using v-text directive",
    };
  }
  
};
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
<!-- this is rleated to main branch-->