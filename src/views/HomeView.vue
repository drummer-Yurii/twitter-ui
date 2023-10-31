<template>
  <div class="home">
    <TheTweet v-for="tweet in tweets" :key="tweet._id" :tweet="tweet" />
  </div>
</template>

<script>
import { ref } from 'vue';
import vweets from '@/vweets';
import TheTweet from '@/components/TheTweet.vue';

export default {
  components: {
    TheTweet
  },
  setup() {
    const tweets = ref(vweets);

    return {
      TheTweet,
      tweets,
    }
  }
}
</script>
