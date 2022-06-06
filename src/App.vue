<template>
  <div id="app">
    <h2>Reading Recorder</h2>
    <!-- メインメニューを定義 -->
    <el-menu mode="horizontal" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
      <el-menu-item index="1">
        <router-link to="/">
          Home
        </router-link>
      </el-menu-item>
      <!-- サブメニューを定義 -->
      <el-submenu index="3">
        <template v-slot:title>Support</template>
        <el-menu-item index="3-1">
          <a href="https://wings.msn.to/" target="help">Author</a>
        </el-menu-item>
        <el-menu-item index="3-2">
          <a href="https://www.sbcr.jp/" target="help">Publisher</a>
        </el-menu-item>
      </el-submenu>
    </el-menu>
    <!-- ルーティング時の表示領域を準備 -->
    <route-view/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
