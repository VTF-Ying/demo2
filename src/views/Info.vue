<template>
  <div>
   hello info component
   <button type="button" @click="add()">添加</button>
  </div>
</template>
<script>
import store from '@/store'
export default {
  name: 'Info',
  // eslint-disable-next-line no-undef
  methods: {
    add () {
      console.log('add Even from info!')
      debugger
      store.commit('increase')
    }
  }
}
</script>
<style scoped>
</style>
