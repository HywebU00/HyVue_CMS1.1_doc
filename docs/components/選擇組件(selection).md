# 選擇組件（Selection）

?> 本範基於 Vuetify3 元件庫 開發 詳細說明請參考 [相關文件](https://vuetifyjs.com/en/#javascript)

<hr style="margin-bottom:3rem;"/>

### 步驟列元件

?> 步驟列元件 詳請請參考[文件連結](https://vuetifyjs.com/en/components/steppers/#usage)

<img  src="doc_img/img_steppers.png"></img>

<h4>引入元件</h4>

```vue
<template>
  <v-stepper v-model="e1" non-linear>
    <template v-slot:default="{ prev, next }">
      <v-stepper-header>
        <template v-for="n in steps" :key="n">
          <v-stepper-item color="primary" :complete="e1 > n" :step="n" :value="n">
            <template #title>
              <div class="title">Name of step {{ n }}</div>
            </template>
            <template #subtitle>
              <div>
                <div class="subtitle">Optional</div>
              </div>
            </template>
          </v-stepper-item>
          <v-divider v-if="n !== steps" :key="n"></v-divider>
        </template>
      </v-stepper-header>

      <v-stepper-window>
        <v-stepper-window-item v-for="n in steps" :key="n" :value="n">
          <v-card>
            <div class="title">Step One</div>
            <div class="text">...</div>
          </v-card>
        </v-stepper-window-item>
      </v-stepper-window>

      <v-stepper-actions>
        <template #prev>
          <v-btn @click="prev" variant="outlined" color="primary">PREVIOUS</v-btn>
        </template>
        <template #next>
          <v-btn color="primary" variant="elevated" @click="next"> NEXT </v-btn>
        </template>
      </v-stepper-actions>
    </template>
  </v-stepper>
</template>
```

<hr style="margin-bottom:8rem;"/>
