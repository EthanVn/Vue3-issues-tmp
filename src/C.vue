<template>C</template>

<script setup lang="ts">
import { defineComponent, onUnmounted } from 'vue'

onUnmounted(() => alert('C-onUnmounted'))
</script>

<script lang="ts">
export default defineComponent({ name: 'C' })
</script>
