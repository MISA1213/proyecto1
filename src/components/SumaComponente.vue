<template>
    <div>
        <h1>Numero1 {{numero1}}</h1>
        <input type="number" v-model="numero1">
        <input type="number" v-model="numero2">

        <button @click="resultado()"> mostrar numero1</button>
    </div>
</template>

<script>
    export default {
 
  data(){
    return{
        numero1: 0,
        numero2: 0,
        total: 0
        
    }
    
}, 
methods:{
    resultado(){
        this.total = Number(this.numero1) + Number(this.numero2)
        console.log('total::: ', this.total);
      //this.total = parseInt(this.numero1) + parseInt(this.numero2)
     // this.total = (+ this.numero1) + ( + this.numero2)
      
      console.log( typeof this.total);
      console.log(  this.total);
    }
  }
}
</script>

<style lang="css" scoped>

</style>