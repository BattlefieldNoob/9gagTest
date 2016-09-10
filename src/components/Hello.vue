<template>
  <div id="feed">
    <div v-for="item in items">
      <p>{{item.caption}}</p>
      <img :src="item.images.normal" />
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {}
  },
  props:{
  items:{
    type:Array,
    default:[]
  }
}   
}
</script>