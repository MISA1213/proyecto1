<template>
  <div class="home">

<h1>{{ titulo }}</h1>
<br>
<SumaComponente/>
    
  </div>
</template>

<script>
import SumaComponente from '@/components/SumaComponente.vue';

export default {
  name: 'Holaiew',
  components: {SumaComponente},
  data(){
    return{

      titulo:'hola este es el Titulo'
    }

  }
}
</script>
