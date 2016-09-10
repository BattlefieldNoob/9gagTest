<template>
  <div id="app">
    <gagFeed :items="images"></gagFeed>
  </div>
</template>

<script>
import gagFeed from './components/Hello.vue'
import request from 'request'
import gag from 'node-9gag'
export default {
  data () {
    return {
      images:[]
    }
  },
  components: {
    gagFeed
  }
}
console.log("popopopopopoop")
/*request("http://infinigag.k3min.eu/hot",function(err,res,body){
        console.log(body)
})*/
gag.section("hot",function(err,res){
  console.log(err)
  console.log(res)
})
</script>

<style>
</style>
