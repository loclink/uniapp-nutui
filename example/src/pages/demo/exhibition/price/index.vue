<script lang="ts">
import { ref } from 'vue'

export default {
  setup() {
    const price = ref(0)
    setInterval(() => {
      price.value = Math.random() * 10000000
      // console.log('price.value1', price.value)
    }, 1000)
    return {
      price,
    }
  },
}
</script>

<template>
  <div class="demo">
    <nut-cell-group title="支持三种尺寸：small、normal、large">
      <nut-cell>
        <nut-price :price="0" size="small" :need-symbol="false" />
      </nut-cell>
      <nut-cell>
        <nut-price :price="0" size="normal" :need-symbol="false" />
      </nut-cell>
      <nut-cell>
        <nut-price :price="0" size="large" :need-symbol="false" />
      </nut-cell>
    </nut-cell-group>
    <h2 class="title">
      不保留小数
    </h2>
    <nut-cell>
      <nut-price :price="8888" :decimal-digits="0" />
    </nut-cell>
    <h2 class="title">
      划线价
    </h2>
    <nut-cell>
      <nut-price :price="8888" :decimal-digits="0" size="normal" need-symbol thousands strike-through />
    </nut-cell>
    <h2 class="title">
      货币符号
    </h2>
    <nut-cell>
      <nut-price :price="10010.01" symbol="¥" />
    </nut-cell>
    <h2 class="title">
      货币符号位置
    </h2>
    <nut-cell>
      <nut-price :price="8888.01" position="after" symbol="元" />
    </nut-cell>
    <h2 class="title">
      千位分隔
    </h2>
    <nut-cell>
      <nut-price :price="15213.1221" :decimal-digits="3" :thousands="true" />
    </nut-cell>
  </div>
</template>

<style lang="scss"></style>

<route lang="json">
{
  "style": {
    "navigationBarTitleText": "Price"
  }
}
</route>
