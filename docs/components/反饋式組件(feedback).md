# 反饋式組件 (feedback)

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 警告框

?> 警告框元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/alert)

<img  src="doc_img/img_containment_alert.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-alert title="Alert title" text="...">
    <template #prepend><span class="material-icons"> info_outline </span> </template>
    <template #close>
      <v-btn variant="text">
        <span class="material-icons"> close </span>
      </v-btn>
    </template>
  </v-alert>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 空狀態元件

?> 空狀態元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/empty-states/#usage)

<img  src="doc_img/img_empty.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-empty-state headline="Whoops, 404" title="Page not found" text="The page you were looking for does not exist">
    <template v-slot:headline>
      <div class="img">
        <v-img src="..."> </v-img>
      </div>
      <div class="title">Whoops, 404</div>
    </template>
  </v-empty-state>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 環狀進度條

?> 環狀進度條 詳請請參考[文件連結](https://vuetifyjs.com/en/components/progress-circular/#color)

<img  src="doc_img/img_progressCri.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-progress-circular model-value="75" class="rounded" color="secondary60" :size="90" :width="6">
    <template v-slot:default>
      <div class="text"><span>75</span>%</div>
    </template>
  </v-progress-circular>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 線性進度條

?> 環狀進度條 詳請請參考[文件連結](https://vuetifyjs.com/en/components/progress-linear/#usage)

<img  src="doc_img/img_progress_liner.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-progress-linear model-value="0" color="primary" rounded :height="14"> </v-progress-linear>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 消息列元件

?> 消息列元件 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/snackbars/)

<img  src="doc_img/img_snackbar.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-snackbar :timeout="2000">
    <template v-slot:activator="{ props }">
      <v-btn color="neutral20" class="ma-2" v-bind="props">open</v-btn>
    </template>
    Hello, I am a snackbar
  </v-snackbar>
</template>
```

<hr style="margin-bottom:8rem;"/>

### 時間軸元件

?> 時間軸元件 詳請請參考[文件連結](https://vuetifyjs.com/zh-Hans/components/timelines/#api)

<img  src="doc_img/img_timeline.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-timeline dot-color="secondary60">
    <v-timeline-item size="small">
      <template v-slot:opposite> Opposite content </template>
      <div>
        <div class="title">
          <span class="material-icons-outlined"> comment </span>
          <span>Content title</span>
        </div>
        <p>...</p>
      </div>
    </v-timeline-item>
    <v-timeline-item>
      <template v-slot:opposite> Opposite content </template>
      <div>
        <div class="title">
          <span class="material-icons-outlined"> comment </span>
          <span> Content title</span>
        </div>
        <p>...</p>
      </div>
    </v-timeline-item>
    <v-timeline-item side="start">
      <template v-slot:opposite> Opposite content </template>
      <template v-slot:icon>
        <span>LC</span>
      </template>
      <div>
        <div class="title">
          <span class="material-icons-outlined"> comment </span>
          <span> Content title</span>
        </div>
        <p>...</p>
      </div>
    </v-timeline-item>
    <v-timeline-item side="end">
      <template v-slot:opposite> Opposite content </template>
      <template v-slot:icon>
        <v-avatar image="@/assets/demo/account.jpg"></v-avatar>
      </template>
      <div>
        <div class="title">
          <span class="material-icons-outlined"> comment </span>
          <span> Content title</span>
        </div>
        <p>....</p>
      </div>
    </v-timeline-item>
    <v-timeline-item side="start">
      <template v-slot:opposite> Opposite content </template>
      <template v-slot:icon>
        <span class="material-icons-outlined"> grade </span>
      </template>
      <div>
        <div class="title">
          <span class="material-icons-outlined"> comment </span>
          <span> Content title</span>
        </div>
        <p>...</p>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>
```

<hr style="margin-bottom:8rem;"/>
