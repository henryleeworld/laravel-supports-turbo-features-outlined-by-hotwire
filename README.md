# Laravel 8 支援 Hotwire 列出的 Turbo 功能

引入 tonysm 的 turbo-laravel 套件來擴增支援 Hotwire 列出的 Turbo 功能，Turbo 提供了一些補充技術，來大幅減少應用程式需要撰寫的 JavaScript，不用大量 JavaScript，而是傳送 HTML 的方式，不只可以實現快速載入首次頁面的目的，還能夠將模板渲染交給伺服器，並在不犧牲傳統單頁應用程式的速度與回應性的情況下，讓開發者使用各種程式語言開發網頁程式，有效提升生產力。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/` 來進行歡迎畫面瀏覽。

----

## 畫面截圖
![](https://i.imgur.com/rGD8064.png)
> Turbo Frames 可以將頁面解構成為獨立的內容，透過定義瀏覽的範圍，並進行延遲載入