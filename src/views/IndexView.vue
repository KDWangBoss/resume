<template>
  <div>
    <div @click="increment">我是标题</div>
    <div>我是计数器：{{ count }}</div>
  </div>
</template>
<script setup>

import { ref, onMounted } from "vue"
const count = ref(0)

// 用来修改状态、触发更新的函数
function increment() {
  count.value++
}

// 生命周期钩子
onMounted(() => {
  console.log(`The initial count is ${count.value}.`)
})

</script>
<style lang="scss" scoped>
.color-red {
  color: red;
}
</style>
