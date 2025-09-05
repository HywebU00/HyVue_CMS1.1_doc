# 容器組件 (containment)

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 按鈕

?> 按鈕組件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/buttons/#usage)

<img  src="doc_img/img_containment_btn.png"></img>

<h4>引入元件</h4>

```vue
尺寸大小
<template>
  <v-btn size="large" color="primary"> Button </v-btn>
  <v-btn color="primary"> Button </v-btn>
  <v-btn size="small" color="primary"> Button </v-btn>
</template>

圓角
<template>
  <v-btn color="primary" size="large" rounded="sm"> radius 4 / SM </v-btn>
  <v-btn color="primary" size="large" rounded="md"> radius 12 / MED </v-btn>
  <v-btn color="primary" size="large" rounded="lg"> radius 24 / LG </v-btn>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 卡片樣式

?> 卡片樣式 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/cards)

<img  src="doc_img/img_card.png"></img>

<h4>引入元件</h4>

```vue
卡片元件樣式
<template>
  <card variant="elevated" />
  <card variant="flat" />
  <card variant="outlined" />
  <card variant="tonal" />
  <card variant="text" />
  <card variant="plain" />
</template>

橫向樣式
<template>
  <card type="list" />
</template>
```

<hr style="margin-bottom:8rem;"/>

### 標籤

?> 標籤樣式 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/chip)

<img  src="doc_img/img_chip.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-chip link label> 標籤 </v-chip>
  <v-chip variant="outlined" link label> 標籤 </v-chip>
  <v-chip variant="elevated" link label> 標籤 </v-chip>
  <v-chip variant="text" link label> 標籤 </v-chip>
  <v-chip variant="plain" link label> 標籤 </v-chip>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 對話框

?> 對話框樣式 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/dialogs)

<img src="doc_img/img_dialogs.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-dialog class="dialogSmall" max-width="350">
    <template v-slot:activator="{ props: activatorProps }">
      <v-btn v-bind="activatorProps" color="primary" text="Open Dialog" variant="flat"></v-btn>
    </template>

    <template v-slot:default="{ isActive }">
      <v-card>
        <v-card-title class="bg-neutral80">
          <span class="material-icons-outlined"> link </span>
          Copy link
        </v-card-title>
        <v-card-text> ... </v-card-text>
        <v-card-actions>
          <v-btn class="closeBtn" text="Close" color="neutral40" @click="isActive.value = false"></v-btn>
          <v-btn variant="outlined" text="..." color="primary"></v-btn>
          <v-btn variant="flat" text="..." color="primary"></v-btn>
        </v-card-actions>
      </v-card>
    </template>
  </v-dialog>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 擴展面板

?> 擴展面板樣式 詳請請參考[文件連結](https://vuetifyjs.com/en/components/expansion-panels/#usage)

<img src="doc_img/img_dialogs.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-expansion-panels>
    <v-expansion-panel>
      <v-expansion-panel-title collapse-icon="mdi-minus" expand-icon="mdi-plus"> Title </v-expansion-panel-title>
      <v-expansion-panel-text> ... </v-expansion-panel-text>
    </v-expansion-panel>
    <v-expansion-panel>
      <v-expansion-panel-title>
        Title
        <template v-slot:actions="{ expanded }">
          <v-icon :color="!expanded ? 'teal' : ''" :icon="expanded ? 'mdi-pencil' : 'mdi-check'"></v-icon>
        </template>
      </v-expansion-panel-title>
      <v-expansion-panel-text> ... </v-expansion-panel-text>
    </v-expansion-panel>
    <v-expansion-panel>
      <v-expansion-panel-title disable-icon-rotate>
        Title
        <template v-slot:actions>
          <v-icon color="error" icon="mdi-alert-circle"> </v-icon>
        </template>
      </v-expansion-panel-title>
      <v-expansion-panel-text> .... </v-expansion-panel-text>
    </v-expansion-panel>
  </v-expansion-panels>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 提示

?> 提示樣式 詳請請參考[文件連結](https://vuetifyjs.com/en/components/tooltip)

<img  src="doc_img/img_tooltip.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-tooltip activator="parent" location="start">prompt text</v-tooltip>
  <v-tooltip activator="parent" location="end">prompt text</v-tooltip>
  <v-tooltip activator="parent" location="top">prompt text</v-tooltip>
  <v-tooltip activator="parent" location="bottom">prompt text</v-tooltip>
</template>
```

<hr style="margin-bottom:8rem;"/>
