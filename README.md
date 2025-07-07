Yuan Chiu的履歷頁面
===

本頁基本上是以Hugo almeida-cv為基礎，針對我的需求客製化處理過。

## 基礎來源
* Hugo <https://gohugo.io/getting-started/installing/>
* almeida-cv <https://github.com/ineesalmeida/almeida-cv>

## 有調整的部份
### 魔改學歷區塊版型
改在
* layouts/partials/_education.html
* assets/scss/components/_education.scss

### 讓網站支援多頁列印
改在 assets/scss/_custom.scss

可惜目前的CSS限制，還不能完美加上頁碼QQ

### 出現可列印提示
改在 assets/scss/_custom.scss

純CSS處理，不對HTML有任何改動，也不注入JS。

## 建置說明
### Start Hugo in development mode
```
hugo server -D
```
Your site is now available at http://localhost:1313/.

### Building
To generate static files of your website, execute the following:
```
hugo --minify
```
within the root of your project.