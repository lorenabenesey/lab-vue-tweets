<template>
  <div className="tweet">
    <img
      :src="image"
      className="profile"
      alt="profile"
    />

    <div className="body">
      <div className="top">
        <span className="user">
          <Name :name ="name"/>
          <span className="handle">@{{ tweet.handle.value }}</span>
        </span>

        <span className="timestamp">{{ tweet.timestamp }}</span>
      </div>

      <p className="message">
        {{ $tweets.message.value }}
      </p>

      <div className="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import Mame from './Name.vue';
const tweet = defineProps(["tweet"]);



</script>
<style scoped>
a {
  color: #42b983;
}
</style>
