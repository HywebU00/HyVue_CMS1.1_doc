# 導覽式組件（Navigation）

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 麵包屑導航

?> 麵包屑導航 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/breadcrumbs/)

<img  src="doc_img/img_bread.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-breadcrumbs :items="['Foo', 'Bar', 'Fizz']" />
  <v-breadcrumbs :items="['Foo', 'Bar', 'Fizz']">
    <template v-slot:prepend>
      <span class="material-symbols-rounded text-neutral40" size="small"> home </span>
    </template>
  </v-breadcrumbs>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 頁籤元件

?> 頁籤元件 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/tabs/#section-4f7f7528)

<img  src="doc_img/img_tab.png"></img>

<h4>引入元件</h4>

```vue
<template>
  tabs
  <v-tabs v-model="tab" class="tabs">
    <v-tab value="one">
      <div class="title">頁籤項目ㄧ</div>
      <template #append>
        <span class="material-icons-outlined"> edit </span>
      </template>
    </v-tab>
    <v-tab value="two">
      <div class="title">頁籤項目ㄧ</div>

      <template #append>
        <span class="material-icons-outlined"> edit </span>
      </template>
    </v-tab>
    <v-tab value="three">
      <div class="title">頁籤項目ㄧ</div>
      <template #append>
        <span class="material-icons-outlined"> edit </span>
      </template></v-tab
    >
  </v-tabs>
  textTab
  <v-tabs v-model="tab2" class="textTabs bg-white" color="primary">
    <v-tab :value="1">
      <div class="title">頁籤項目ㄧ</div>
    </v-tab>
    <v-tab :value="2">
      <div class="title">頁籤項目ㄧ</div>
    </v-tab>
    <v-tab :value="3">
      <div class="title">頁籤項目ㄧ</div>
    </v-tab>
  </v-tabs>
</template>
```

<hr style="margin-bottom:8rem;"/>
