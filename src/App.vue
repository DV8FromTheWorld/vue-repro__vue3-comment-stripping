<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <br />Demo code starts in the App.vue file.
    <br />If there is something to display it will appear below here.

    <ErrorBoundary>
      <SlottableComponent>
        <!-- Comment that should be stripped -->
        <div>
          Hello World!
        </div>
        <!-- Another comment to strip out -->
      </SlottableComponent>
    </ErrorBoundary>
  </div>
</template>

<script>
  import ErrorBoundary from './components/ErrorBoundary'

  import SlottableComponent from './components/SlottableComponent'

  export default {
    name: 'App',
    components: {
      ErrorBoundary,
      SlottableComponent
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
