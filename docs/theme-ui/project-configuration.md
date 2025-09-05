# 專案配置

## Color

?> 要更改主要顏色和相關色系設定如下：

### 覆蓋主題顏色

如需更改，請前往： src/plugins/vuetify.js <br/>
預設主題色為 default 設定

### 更改主題顏色

如需更改切換的主題色彩及暗黑設定，請前往： src/plugins/vuetify.js <br/>
至對應的主題色更改設定，欲新增主題色彩 也可自定義主題名稱

```javascript
 theme: {
    defaultTheme: "default",
    themes: {
      default: {
        dark: false,
        colors: {
          // primary 設定
          primary: "#014d92", //$primary30
          primary50: "#0463b8", //$primary50
          primary70: "#f6fbff", //$primary70
          //secondary 設定
          secondary: "#2d62b3", //secondary40
          "secondary-lighten-0": "#0055A0",
          secondary60: "#057bb7", //secondary60
          secondary80: "#80cbd7", //secondary80
          secondary100: "#ebf0f9", //secondary100
          //Neutral 設定
          neutral: "#ffffff", //Neutral100
          neutral80: "#F8F8F8", //Neutral80
          neutral70: "#F1F1F1", //Neutral70
          neutral60: "#DEE0E3", //Neutral60
          neutral40: "#97A3B6", //Neutral40
          neutral30: "#69707D", //Neutral30
          neutral20: "#555555", //Neutral20
          neutral10: "#333333", //Neutral10
          //Success 設定
          success: "#00754B", //Green30
          "success-lighten-1": "#EEF8E4", //Green70
          //Info 設定
          info: "#00529B", //blue30
          "info-lighten-1": "#E7F3FF", //blue70
          //warning 設定
          warning: "#C23E00", //warning30
          "warning-lighten-1": "#FAECE6", //warning70
          //Error 設定
          error: "#C40000", //red30
          "error-lighten-1": "#FFEDF1", //red70
          light: "#36e79e",
          //thead
          thead: "#057bb7", //secondary60,
        },
      },
      green: {
        dark: false,
        colors: {
          // primary 設定
          primary: "#1f7848", //$primary30
          primary50: "#44aa55", //$primary50
          primary70: "#e5f7eb", //$primary70
          //secondary 設定
          secondary: "#1ab64c", //secondary40
          secondary60: "#33a59c", //secondary60
          secondary80: "#86d9bc", //secondary80
          secondary100: "#f2fbf6", //secondary100
          //Neutral 設定
          neutral: "#ffffff", //Neutral100
          neutral80: "#F8F8F8", //Neutral80
          neutral70: "#F1F1F1", //Neutral70
          neutral60: "#DEE0E3", //Neutral60
          neutral40: "#97A3B6", //Neutral40
          neutral30: "#69707D", //Neutral30
          neutral20: "#555555", //Neutral20
          neutral10: "#333333", //Neutral10
          //Success 設定
          success: "#00754B", //Green30
          "success-lighten-1": "#EEF8E4", //Green70
          //Info 設定
          info: "#00529B", //blue30
          "info-lighten-1": "#E7F3FF", //blue70
          //warning 設定
          warning: "#C23E00", //warning30
          "warning-lighten-1": "#FAECE6", //warning70
          //Error 設定
          error: "#C40000", //red30
          "error-lighten-1": "#FFEDF1", //red70
          light: "#86d9bc",
          //thead
          thead: "#33a59c", //secondary60
        },
      },
      purple: {
        dark: false,
        colors: {
          // primary 設定
          primary: "#8e0d70", //$primary30
          primary50: "#cf3eab", //$primary50
          primary70: "#f8ebf6", //$primary70
          //secondary 設定
          secondary: "#911a76", //secondary40
          secondary60: "#ce3d86", //secondary60
          secondary80: "#dd6081", //secondary80
          secondary100: "#fff2fa", //secondary100
          //Neutral 設定
          neutral: "#ffffff", //Neutral100
          neutral80: "#F8F8F8", //Neutral80
          neutral70: "#F1F1F1", //Neutral70
          neutral60: "#DEE0E3", //Neutral60
          neutral40: "#97A3B6", //Neutral40
          neutral30: "#69707D", //Neutral30
          neutral20: "#555555", //Neutral20
          neutral10: "#333333", //Neutral10
          //Success 設定
          success: "#00754B", //Green30
          "success-lighten-1": "#EEF8E4", //Green70
          //Info 設定
          info: "#00529B", //blue30
          "info-lighten-1": "#E7F3FF", //blue70
          //warning 設定
          warning: "#C23E00", //warning30
          "warning-lighten-1": "#FAECE6", //warning70
          //Error 設定
          error: "#C40000", //red30
          "error-lighten-1": "#FFEDF1", //red70
          light: "#dd6081",
          //thead
          thead: "#ce3d86", //secondary60
        },
      },
      red: {
        dark: false,
        colors: {
          // primary 設定
          primary: "#91404A", //$primary30
          primary50: "#b6636E", //$primary50
          primary70: "#f6e8ed", //$primary70
          //secondary 設定
          secondary: "#ad3b5f", //secondary40
          secondary60: "#c88490", //secondary60
          secondary80: "#e6c9cc", //secondary80
          secondary100: "#ebf0f9", //secondary100
          //Neutral 設定
          neutral: "#ffffff", //Neutral100
          neutral80: "#F8F8F8", //Neutral80
          neutral70: "#F1F1F1", //Neutral70
          neutral60: "#DEE0E3", //Neutral60
          neutral40: "#97A3B6", //Neutral40
          neutral30: "#69707D", //Neutral30
          neutral20: "#555555", //Neutral20
          neutral10: "#333333", //Neutral10
          //Success 設定
          success: "#00754B", //Green30
          "success-lighten-1": "#EEF8E4", //Green70
          //Info 設定
          info: "#00529B", //blue30
          "info-lighten-1": "#E7F3FF", //blue70
          //warning 設定
          warning: "#C23E00", //warning30
          "warning-lighten-1": "#FAECE6", //warning70
          //Error 設定
          error: "#C40000", //red30
          "error-lighten-1": "#FFEDF1", //red70
          light: "#e6c9cc",
          //thead
          thead: "#c88490", //secondary60,
        },
      },
      dark: {
        dark: true,
        colors: {
          primary: "#fefefe",
          secondary: "#695f5f",
          light: "#33a59c",
          thead: "#555555",
        },
      },
    },
  }


```

### 修改字型樣式

如需修改文字樣式則須至 src / sass / variables.scss

```sass
$fontFamily: 'Noto Sans', 'Noto Sans TC', Lato, 'PingFang TC', 'Helvetica Neue', Helvetica, 微軟正黑體, Arial, sans-serif;
```

## Icons

?> 要更改 Icons 主題及樣式 如下：

### 自行設定 icon

可依照檔案需求，載入所需的 Icon 類型<br>
src / plugins / vuetify.js

> 類型樣式 可參考 [Vuetify 文件](https://vuetifyjs.com/en/features/icon-fonts/#material-icons-css)

```javascript
icons: {
    defaultSet: "mdi",
    aliases,
    sets: {
      fa,
      mdi,
    },
  },
```

### 可外部自行載入 icon

檔案放置位子如下： <br/>
sass / vendor / material-icons-round.scss <br/>
sass / setting.scss <br/>

> 撰寫及載入方式可參閱[ Google Fonts](https://fonts.google.com/icons)

```sass
//material-icons-round
@import '@/sass/vendor/material-icons-round.scss';
```

```html
<span class="material-icons-round"> logout </span>
```

## 響應式斷點

### 使用

此模板 根據 [Vuetify](https://vuetifyjs.com/zh-Hans/components/grids/#section-4f7f7528) 的配置設定。使用 flexbox 建構的 12 格網格系統。網格用於在應用程式的定的佈局。
<br/>包含 5 種斷點來針對特定的螢幕尺寸或方向：xs、sm、md、lg 和 xl。可以透夠需求來調整斷點尺寸。<br/>

> 各元件也可透過 sass 的設定 來調整各斷點的樣式，相關變數連結為：
> sass/common/ mixins/ \_mediaquery.scss

| 裝置     | 名稱 | 類型                   | 範圍              |
| -------- | ---- | ---------------------- | ----------------- |
| 超小尺寸 | xs   | Small to large phone   | < 600px           |
| 小尺寸   | sm   | Small to medium tablet | 600px > < 960px   |
| 中尺寸   | md   | Large tablet to laptop | 960px > < 1280px  |
| 大尺寸   | lg   | Laptop to desktop      | 1280px > < 1920px |
| 超大尺寸 | xl   | 1080p to 1440p desktop | 1920px > < 2560px |
| 超大尺寸 | xxl  | 4k and ultra-wide      | > 2560px          |
