<template>
  <div>
    <h1>首页</h1>
    <p>{{ store.state.count }}</p>
    <p>{{ $store.state.count }}</p>
  </div>
</template>

<script setup lang="ts">
import User from '@/api/User'
// import { useStore } from 'vuex'
import { useStore } from '../../store/index'

const store = useStore()
console.log(store.state.count)
console.log(User)

</script>

<style lang="scss" scoped>
h1{
  color:$injectedColor;
}
</style>
