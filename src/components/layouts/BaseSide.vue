<script lang="ts" setup>
import { Menu as IconMenu } from '@element-plus/icons-vue'

// const isCollapse = ref(true)
function handleOpen(key: string, keyPath: string[]) {
  // eslint-disable-next-line no-console
  console.log(key, keyPath)
}
function handleClose(key: string, keyPath: string[]) {
  // eslint-disable-next-line no-console
  console.log(key, keyPath)
}
</script>

<template>
  <el-menu
    router
    default-active="1"
    class="el-menu-vertical-demo"
    @open="handleOpen"
    @close="handleClose"
  >
    <el-menu-item index="/ag-grid">
      <el-icon>
        <IconMenu />
      </el-icon>
      <template #title>
        AG Grid
      </template>
    </el-menu-item>
  </el-menu>
</template>
