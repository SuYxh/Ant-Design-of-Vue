<template>
  <a-layout id="components-layout-demo-top-side-2">
    <a-layout-header class="header">
      <div class="logo" />
      <a-menu
        theme="dark"
        mode="horizontal"
        :default-selected-keys="['2']"
        :style="{ lineHeight: '64px' }"
      >
        <a-menu-item key="1">
          nav 1
        </a-menu-item>
        <a-menu-item key="2">
          nav 2
        </a-menu-item>
        <a-menu-item key="3">
          nav 3
        </a-menu-item>
      </a-menu>
    </a-layout-header>
    <a-layout>
      <!-- 侧边栏 -->
      <a-layout-sider width="200" style="background: #fff">
        <a-menu
          mode="inline"
          theme="dark"
          :default-selected-keys="['0']"  
          :style="{ height: '100%', borderRight: 0 }"
        >
          <a-menu-item key="0" >
              首页
            </a-menu-item>
          <a-sub-menu key="sub1">
            <span slot="title"><a-icon type="user" />Navigation</span>
            <a-menu-item key="1" >
              面包屑
            </a-menu-item>
            <a-menu-item key="2">
              下拉菜单
            </a-menu-item>
            <a-menu-item key="3">
              分页
            </a-menu-item>
            <a-menu-item key="4">
              步骤条
            </a-menu-item>
          </a-sub-menu>
          <a-sub-menu key="sub2">
            <span slot="title"><a-icon type="laptop" />表单</span>
            <a-menu-item key="5">
              option5
            </a-menu-item>
            <a-menu-item key="6">
              option6
            </a-menu-item>
            <a-menu-item key="7">
              option7
            </a-menu-item>
            <a-menu-item key="8">
              option8
            </a-menu-item>
          </a-sub-menu>
          <a-sub-menu key="sub3">
            <span slot="title"><a-icon type="notification" />表格</span>
            <a-menu-item key="9">
              option9
            </a-menu-item>
            <a-menu-item key="10">
              option10
            </a-menu-item>
            <a-menu-item key="11">
              option11
            </a-menu-item>
            <a-menu-item key="12">
              option12
            </a-menu-item>
          </a-sub-menu>
        </a-menu>
      </a-layout-sider>
      <!-- 面包屑 -->
      <a-layout style="padding: 0 24px 24px">
        <a-breadcrumb style="margin: 16px 0">
          <a-breadcrumb-item>Home</a-breadcrumb-item>
        </a-breadcrumb>
        <!-- 卡片区域 -->
        <a-layout-content
          :style="{ background: '#fff', padding: '24px 90px', margin: 0, minHeight: '280px' }"
        >
          <img src="../assets/antd.png" alt="antd">
          <img src="../assets/vue.png" alt="antd">
          <img src="../assets/antd.png" alt="antd">
        </a-layout-content>
      </a-layout>
    </a-layout>
  </a-layout>
</template>
<script>
export default {
  data() {
    return {
      collapsed: false,
    };
  },
};
</script>

<style>
.ant-layout{
  height: 100%;
}
#components-layout-demo-top-side-2 .logo {
  width: 120px;
  height: 31px;
  background: rgba(255, 255, 255, 0.2);
  margin: 16px 28px 16px 0;
  float: left;
}
</style>
