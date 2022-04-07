<script setup>
import { NAvatar } from 'naive-ui'
import { NConfigProvider, NGlobalStyle, darkTheme } from 'naive-ui';
darkTheme 
</script>

<template>
<NConfigProvider :theme="darkTheme">
<n-global-style />
  <n-avatar
  round
  size="small"
  src="https://07akioni.oss-cn-beijing.aliyuncs.com/07akioni.jpeg"
  ></n-avatar>


  <h1>Hello App!</h1>
  <p>
    <!--使用 router-link 组件进行导航 -->
    <!--通过传递 `to` 来指定链接 -->
    <!--`<router-link>` 将呈现一个带有正确 `href` 属性的 `<a>` 标签-->
    <router-link to="/">Go to Home</router-link>
    <!-- <router-link to="/about">Go to About</router-link> -->
  </p>
  <!-- 路由出口 -->
  <!-- 路由匹配到的组件将渲染在这里 -->
  <router-view></router-view>
</NConfigProvider>
</template>

<style>

</style>
