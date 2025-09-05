# 圖像和圖標組件 (Images & icons)

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 頭像元件

?> 頭像元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/avatars/#usage)

<img  src="doc_img/img_avatars.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-avatar rounded="sm" class="bg-neutral30">
    <span class="material-icons-outlined"> person </span>
  </v-avatar>
  <v-avatar class="bg-neutral30" rounded="full">
    <span class="material-icons-outlined"> person </span>
  </v-avatar>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 圖標元件

?> 圖標元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/icons/#usage)

<img  src="doc_img/img_icon.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-icon color="info" size="30" icon="mdi-information"></v-icon>
  <v-icon color="success" size="30" icon="mdi-information"></v-icon>
  <v-icon color="warning" size="30" icon="mdi-information"></v-icon>
  <v-icon color="error" size="30" icon="mdi-information"></v-icon>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 圖像元件

?> 圖像元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/images/#usage)

<img  src="doc_img/img_img.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-img rounded="md" :width="300" :aspect-ratio="1 / 1" cover src="@/assets/demo/..."></v-img>
  <v-img rounded="md" :width="300" :aspect-ratio="3 / 2" cover src="@/assets/demo/..."></v-img>
  <v-img rounded="md" :width="300" :aspect-ratio="4 / 3" cover src="@/assets/demo/..."></v-img>
  <v-img rounded="md" :width="300" :aspect-ratio="3 / 1" cover src="@/assets/demo/..."></v-img>
</template>
```

<hr style="margin-bottom:8rem;"/>
