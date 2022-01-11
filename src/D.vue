<template>D</template>

<script setup lang="ts">
import { onUnmounted, defineComponent } from 'vue'

onUnmounted(() => alert('A-onUnmounted'))
</script>

<script lang="ts">
export default defineComponent({ name: 'D' })
</script>
