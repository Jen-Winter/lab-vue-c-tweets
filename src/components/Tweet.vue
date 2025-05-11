<template>
  <div class="tweet">
   <ProfileImage :image="user.image" />

    <!--<div class="body">
      <div class="top">
        <User userData="user"></User>-->

       <!-- <span class="timestamp"></span>
      </div>

      <p class="message">
        
      </p>

      <div class="actions">
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>-->
      <!--</div>
    </div>-->

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>

import ProfileImage from './ProfileImage.vue'

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
})

const { user, timestamp, message } = props.tweet;

 /*const props = defineProps({
  name : {
    type: String,
    required: true
  },
  handle : {
    type: String,
    required: true
  },
  img : {
    type: String,
    required: true
  },
  timestamp : {
    type: String,
    required: true
  },
  message : {
    type: String,
    required: true
  }
})*/
</script>
