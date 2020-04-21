<template lang="html">
  <div class="app">

      <h1>Twitter</h1>
      <section>
        <div class="tweet" v-for="tweet in tweets">
          <h2>{{tweet.name}}</h2>
          <h3>{{tweet.handle}}</h3>
          <img v-bind:src=" tweet.img" />
          <p>Tweet:{{tweet.tweet}}</p>
          <p>Likes:{{tweet.likes}}</p>
        </div>
      </section>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
  return {
    tweets:[
      {
        id: 1,
        name: 'James',
        handle: '@jokerjames',
        img: 'https://semantic-ui.com/images/avatar2/large/matthew.png',
        tweet: "If you don't succeed, dust yourself off and try again.",
        likes: 10,
      },
      {
        id: 2,
        name: 'Fatima',
        handle: '@fantasticfatima',
        img: 'https://semantic-ui.com/images/avatar2/large/molly.png',
        tweet: 'Better late than never but never late is better.',
        likes: 12,
      },
      {
        id: 3,
        name: 'Xin',
        handle: '@xeroxin',
        img: 'https://semantic-ui.com/images/avatar2/large/elyse.png',
        tweet: 'Beauty in the struggle, ugliness in the success.',
        likes: 18,
      }
    ]
  };
},
// computed:{
//   totalTweets: function(){
//     return this.tweets.map((tweet) =>{return tweet.likes});
//    }
// }
}
</script>

<style lang="css" scoped>
</style>
