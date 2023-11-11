<template>
  <view>
    <view v-if="loading">
      loading
    </view>
    <slot v-else></slot>
  </view>
</template>

<script setup>
defineProps({
  loading: {
    type: Boolean,
    default: false,
  }
})
</script>
