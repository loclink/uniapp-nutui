<script setup lang="ts">
import { useAppStore } from '@/store'

const { darkMode } = storeToRefs(useAppStore())
</script>

<template>
  <div class="demo full">
    <h2 class="title">
      基础用法
    </h2>
    <nut-grid>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      自定义列数
    </h2>
    <nut-grid :column-num="3">
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      正方形格子
    </h2>
    <nut-grid :column-num="3" square>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      格子间距
    </h2>
    <nut-grid :gutter="10">
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      内容翻转
    </h2>
    <nut-grid reverse>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      内容横向
    </h2>
    <nut-grid direction="horizontal">
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      图标颜色/大小
    </h2>
    <nut-grid :column-num="3">
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon name="dongdong" size="40px" custom-color="#478EF2" />
      </nut-grid-item>
      <nut-grid-item text="文字">
        <nut-icon :custom-color="darkMode ? '#fff' : '#000'" name="dongdong" />
      </nut-grid-item>
    </nut-grid>

    <h2 class="title">
      页面导航
    </h2>
    <nut-grid :column-num="2">
      <nut-grid-item icon="home" text="路由跳转 ’/‘ " to="/" />
      <nut-grid-item icon="search" text="URL 跳转" url="https://jd.com" />
    </nut-grid>

    <h2 class="title">
      自定义内容
    </h2>
    <nut-grid :border="false">
      <nut-grid-item v-for="i in 4" :key="i">
        <nut-avatar size="large">
          <img
            src="https://img12.360buyimg.com/imagetools/jfs/t1/143702/31/16654/116794/5fc6f541Edebf8a57/4138097748889987.png"
          >
        </nut-avatar>
      </nut-grid-item>
    </nut-grid>
  </div>
</template>

<route lang="json">
{
  "style": {
    "navigationBarTitleText": "Grid"
  }
}
</route>
