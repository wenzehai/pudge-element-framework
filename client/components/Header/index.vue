<template>
<header>
    <el-menu theme="dark" mode="horizontal">
        <el-menu-item class="header-navicon" index="1">
            <el-button type="text" @click="openSidebar">
                <!--<i class="md-icon">menu</i>-->
                <img src="../../assets/img/ico_menu.png" class="md-icon">
            </el-button>
        </el-menu-item>
        <span class="header-title">{{title}}</span>
        <el-submenu class="header-menu" index="3">
            <template slot="title">个人选项</template>
                <el-menu-item index="4-1">个人中心</el-menu-item>
                <el-menu-item index="4-2">帮助文档</el-menu-item>
                <el-menu-item index="4-3">意见反馈</el-menu-item>
                <el-menu-item index="4-4">注销</el-menu-item>
            </el-submenu>
        </el-menu>
    </header>
</template>

<script>
export default {
  name: 'Header',
  props: ['openSidebar', 'title']
}
</script>

<style lang="scss">
// You can import all your SCSS variables using webpack alias
@import '~scss_vars';
@import './style.scss';
</style>
