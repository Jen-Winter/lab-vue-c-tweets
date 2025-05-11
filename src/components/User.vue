<template>
    <span class="user">
        <span class="name">{{ tweet.Userdata.name }}</span>
        <span class="handle">{{ tweet.Userdata.handle }}</span>
    </span>
</template>

<script setup>
const props = defineProps({
  userData: {
    type: Object,
    required: true
  }
})
</script>