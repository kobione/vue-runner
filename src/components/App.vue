<template>
  <div id="app">

    <img src="../assets/images/logo.png" height="100" alt="">
    <h1>{{ firstVariable }}</h1>

    <p>Your first component is has your HTML, CSS, and JavaScript all in one <strong>"single page component"</strong> file.</p>
    <br>

    <p>
      Edit your first "single page component" at:
      <h2><code>./src/components/App.vue</code></h2>
      <strong>Note:</strong> When you "<em>save</em>" in your editor, your browser will <em>automatically reload</em> (thanks to Webpack).
    </p>
    <br>

    <p>{{ thatsIt() }}</p>

  </div>
</template>

<style>
  body {
    text-align: center;
    font-family: Helvetica, sans-serif;
  }
</style>


<script>

  export default {
    data () {
      return {
        firstVariable: 'Hello World!',
      }
    },
    methods: {
      thatsIt: function() {
        return "Goodbye!"
      }
    }
  }

</script>
