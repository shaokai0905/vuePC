<template>
  <div>
    <Header></Header>
    <router-view></router-view>
    <Footer v-show="!$route.meta.isHideFooter"></Footer>
  </div>
</template>

<script>
import Header from './components/Header'
import Footer from './components/Footer'
// import {getCategoryList} from './api'
export default {
  name: 'App',
  mounted () {
    // 异步获取三级分类列表
    // getCategoryList().then(result => {
    //   console.log('result', result)
    // })
    this.$store.dispatch('getCategoryList')
  },
  components:{
    Header,
    Footer
  }
}
</script>

<style scoped>

</style>
