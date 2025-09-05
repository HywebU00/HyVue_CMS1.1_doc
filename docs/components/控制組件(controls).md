# 控制組件 (controls)

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 滑桿元件

?> 滑桿元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/slider)

<img  src="doc_img/img_slider.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-slider color="secondary" v-model="media" hide-details="auto" track-color="neutral60">
    <template v-slot:prepend>
      <span class="material-icons-round text-neutral20"> volume_up </span>
    </template>
  </v-slider>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 範圍滑桿

?> 滑桿元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/range-sliders/#usage)

<img  src="doc_img/img_range.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-range-slider v-model="value" strict track-color="neutral60" color="secondary"></v-range-slider>
</template>
```

<hr style="margin-bottom:8rem;"/>
