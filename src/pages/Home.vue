<template>
  <div class="home">
    <h1>{{ msg }}</h1>
    <Navbar />
  </div>
</template>

<script>
import Navbar from '../components/Navbar';
export default {
  name: 'Home',
  data: function(){
    return {
      
    }
  },
  props: {
    msg: String
  },
  components:{
    Navbar
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.home{

}
</style>
