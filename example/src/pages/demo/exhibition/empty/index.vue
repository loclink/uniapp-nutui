<script lang="ts">
import { ref } from 'vue'

export default {
  setup() {
    const tabValue = ref(0)
    return {
      tabValue,
    }
  },
}
</script>

<template>
  <div class="demo">
    <h2 class="title">
      基础用法
    </h2>
    <div class="show">
      <nut-empty description="无数据" />
    </div>

    <h2 class="title">
      图片类型，内置3个
    </h2>
    <div class="show">
      <nut-tabs v-model="tabValue">
        <nut-tab-pane title="无内容">
          <nut-empty image="empty" description="无内容" />
        </nut-tab-pane>
        <nut-tab-pane title="加载失败/错误">
          <nut-empty image="error" description="加载失败/错误" />
        </nut-tab-pane>
        <nut-tab-pane title="无网络">
          <nut-empty image="network" description="无网络" />
        </nut-tab-pane>
      </nut-tabs>
    </div>

    <h2 class="title">
      自定义图片
    </h2>
    <div class="show">
      <nut-empty description="无优惠券">
        <template #image>
          <img src="https://static-ftcms.jd.com/p/files/61a9e3313985005b3958672e.png">
        </template>
      </nut-empty>
    </div>

    <h2 class="title">
      底部内容
    </h2>
    <div class="show">
      <nut-empty image="error" description="加载失败">
        <div style="margin-top: 10px">
          <nut-button icon="refresh" type="primary">
            重试
          </nut-button>
        </div>
      </nut-empty>
    </div>
  </div>
</template>

<style lang="scss">

</style>

<route lang="json">
{
  "style": {
    "navigationBarTitleText": "Empty"
  }
}
</route>
