<template>
  <div>
    <h1>首页</h1>
    <p>{{ store.state.count }}</p>
    <p>{{ $store.state.count }}</p>
  </div>
</template>

<script setup lang="ts">
// import { useStore } from 'vuex'
import { useStore } from '../../store/index'

const store = useStore()
console.log(store.state.count)

</script>

<style lang="scss" scoped>
</style>
