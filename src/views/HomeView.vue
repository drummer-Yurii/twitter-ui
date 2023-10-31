<template>
  <div class="home">
    <Tweet />
  </div>
</template>

<script>
import { ref } from 'vue';
import vweets from '@/vweets';

export default {
  setup() {
    const tweets = ref(vweets);

    return {
      tweets,
    }
  }
}
</script>
