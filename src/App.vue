<template>
  <div id="app">
    <Redes></Redes>
  </div>

</template>

<script>
import TimeLine from './TimeLine.vue'
import Redes from './redes_s.vue'

export default {
  name: 'app',
  data () {
  },
  components:{
    'TimeLine' : TimeLine,
    'Redes' : Redes
  }

}
</script>

