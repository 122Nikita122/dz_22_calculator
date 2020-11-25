<template>
  <div class="hello">
    <div id="app">
        <input type="text" v-model="x">
        <input type="text" v-model="y">
        <div class="result" v-text="result"></div>
        <button v-on:click="getRandom">Посмотреть рандомное число из вычисленных</button>
        <h3 >Случайное число {{random}}</h3>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Calculator',
      data() {
          return {
            x: 0,
            y: 0,            
            random: 0,
          };      
        },
    computed: {
        result(){
            if(Number.isNaN(+this.x) || Number.isNaN(+this.y)) return  "Вы ввели не число"            
            return  +this.x + +this.y; 
        }
    }, 
    methods: {
        getRandom(){
            if(Number.isNaN(+this.x) || Number.isNaN(+this.y)) return  this.random = "Вы ввели не число" 
            return this.random = Math.floor( Math.random() * (+this.x + +this.y))          
        }
    }
}


</script>
