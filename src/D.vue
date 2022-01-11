<template>D</template>

<script setup lang="ts">
import { onUnmounted, defineComponent } from 'vue'

onUnmounted(() => alert('D-onUnmounted'))
</script>

<script lang="ts">
export default defineComponent({ name: 'D' })
</script>
