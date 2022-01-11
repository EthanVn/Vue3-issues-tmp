<template>
    <KeepAlive include="A,B">
        <component :is="componentOne"></component>
    </KeepAlive>
    <hr />
    <button @click="componentOne = A">SwitchA</button>
    <button @click="componentOne = B">SwitchB</button>

    <hr />
    <hr />
    <hr />

    <KeepAlive include="C,D">
        <component :is="componentTwo"></component>
    </KeepAlive>
    <hr />
    <button @click="componentTwo = C">SwitchC</button>
    <button @click="componentTwo = D">SwitchD</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import A from './A.vue'
import B from './B.vue'
import C from './C.vue'
import D from './D.vue'

const componentOne = ref(A)
const componentTwo = ref(C)
</script>
