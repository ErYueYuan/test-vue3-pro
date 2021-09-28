<template>
  <div></div>
</template>

<script>
import { reactive, toRefs, onBeforeMount, onMounted } from 'vue'
export default {
  name: '',
  //steup 有两个参数props，contenxt进行操作，
  setup(props,context) {
    //需要结构props时使用toRefs，直接结构props话会失去双向数据绑定的功能性
    console.log('1-开始创建组件-setup')
    const data = reactive({})
    onBeforeMount(() => {
      console.log('2.组件挂载页面之前执行----onBeforeMount')
    })
    onMounted(() => {
      console.log('3.-组件挂载到页面之后执行-------onMounted')
    })
    return {
    }
  },
}

</script>
<style scoped lang='less'>
</style>