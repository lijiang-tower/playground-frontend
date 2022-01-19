<template>
  <div id="nav">
    <router-link to="/">Home</router-link>|
    <router-link to="/about">About</router-link>
    <el-row>
      <el-button>button</el-button>
      <el-button :icon="Search" circle></el-button>
      <el-button type="primary" :icon="Edit" circle></el-button>
      <el-button type="success" :icon="Check" circle></el-button>
      <el-button type="info" :icon="Message" circle></el-button>
      <el-button type="warning" :icon="Star" circle></el-button>
      <el-button type="danger" :icon="Delete" circle></el-button>
    </el-row>
  </div>
  <router-view />
</template>

<script lang="ts" setup>
import {
  Search,
  Edit,
  Check,
  Message,
  Star,
  Delete,
} from '@element-plus/icons-vue'

</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
