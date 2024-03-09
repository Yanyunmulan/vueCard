<template>
  <div class="home">
    <app-bar title="INTEREST" left="home" right="search" @left="handleLeftClick" @right="handleRightClick" />
    <tab-list />
    <card-list />
    <card-detail />
  </div>
</template>

<script>
import AppBar from '../components/AppBar.vue'
import TabList from '../components/TabList.vue'
import CardList from '../components/CardList.vue'
import CardDetail from '../components/CardDetail.vue'
export default {
  components: {
    AppBar,
    TabList,
    CardList,
    CardDetail
  },
  // data() {
  //   return {
  //     pageTitle: 'My Page'
  //   };
  // },
  methods: {
    handleLeftClick() {
      // 处理左侧点击事件的逻辑
      console.log('Left button clicked!');
    },
    handleRightClick() {
      // 处理左侧点击事件的逻辑
      console.log('Right button clicked!');
    },
  }
}
</script>

<style lang="scss">
.home {
  height: 100%;
  width: 100%;
  overflow: hidden;
  color: white;
  background-image: linear-gradient(to top, #99acbe 5%, #a8b3bf 20%, #cfd7dd);
}
</style>
