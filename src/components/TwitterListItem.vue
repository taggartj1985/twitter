<template lang="html">
  <div class="">
  <h2>{{tweet.name}}</h2>
  <h3>{{tweet.handle}}</h3>
  <img v-bind:src=" tweet.img" />
  <p>Tweet:{{tweet.tweet}}</p>
  <p>Likes:{{tweet.likes}}</p>
  </div>
</template>

<script>
export default {
  name: 'twitter-list-item',
  props: ['tweet'],
}
</script>

<style lang="css" scoped>
</style>
