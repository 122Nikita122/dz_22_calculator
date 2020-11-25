<template>
  <div id="app">    
    <Calculator/>
    <Watch/>
  </div>
</template>

<script>
import Calculator from './components/Calculator';
import Watch from './components/Watch';

export default {
  name: 'App',
  components: {
    Calculator,
    Watch    
  }
}
</script>

<style>

</style>
