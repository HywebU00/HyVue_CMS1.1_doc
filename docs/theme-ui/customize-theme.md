# 客製化主題

## SCSS 配置

?> 當需要修改模板樣式時

檔案位置如:src/sass<br/>

```text
├── sass/
   ├── common/
   │   └── mixins/
   │   │     ├── _mediaquery.scss     // 相關mixin
   │   │     ├── _scrollbar.scss
   │   │     └── _text.scss
   │   │
   │   ├──  customize_color.scss      // 設定自訂顏色主題 css
   │   ├──  customize_dark.scss       // 設定自訂黑色主題 css
   │   ├──  customize_font.scss       // 設定自訂文字大小 css
   │   └──  customize_shadow.scss     // 設定陰影 css
   │
   ├── components/                    // 元件修改 css
   │   └── ...
   │
   ├── layout/                        // 基本模板頁面 css
   │   └── ...
   │
   ├── vendor/
   │   ├── iconfont                   // googlefont 檔案資料中
   │   └── material-icons-round.scss  // googlefont css
   │
   ├── variables.scss                 // 變數
   └── settings.scss                  // 統一匯出之主要SCSS


```

## 模板功能設定

### 切換主題色彩

?> 當需要修改切換主題顏色配置功能時

檔案位置如:src/components/functionNavigation.vue <br/>
若需要更詳細文件 可參考 [ Vuetify Theme ](https://vuetifyjs.com/en/features/theme/#changing-theme)

```vue
<template>
  <v-btn @click="changeTheme('default')">button</v-btn>
</template>
<script>
export default {
  methods: {
    changeTheme(color) {
      const theme = this.$vuetify.theme;
      theme.change(color);
      this.theme = color;
      this.themeDark = false;
      // 寫入 cookie
      this.createCookie('Theme', color, 356);
    },
    createCookie(name, value, days) {
      let _expires;
      const _date = new Date();
      if (days) {
        _date.setTime(_date.getTime() + days * 24 * 60 * 60 * 1000);
        _expires = '; expires=' + _date.toGMTString();
      } else {
        _expires = '';
      }
      document.cookie = name + '=' + value + _expires + '; path=/';
    },
  },
};
</script>
```

### 切換字體大小

?> 當需要修改切換主題顏色配置功能時

檔案位置如:src/components/functionNavigation.vue <br/>

```vue
<template>
  <v-btn @click="fontSizeChange('medium')"> 中 </v-btn>
</template>
<script>
export default {
  methods: {
    changeFontSizeClass(targetName) {
      const body = document.querySelector('body');
      switch (targetName) {
        case 'small':
          body.classList.remove('largeSize', 'mediumSize');
          body.classList.add('smallSize');
          this.fontSize = 'small';
          break;
        case 'medium':
          body.classList.remove('smallSize', 'largeSize');
          body.classList.add('mediumSize');
          this.fontSize = 'medium';
          break;
        case 'large':
          body.classList.remove('smallSize', 'mediumSize');
          body.classList.add('largeSize');
          this.fontSize = 'large';
          break;
      }
      this.getFontSizeText(targetName);
    },
  },
};
</script>
```
