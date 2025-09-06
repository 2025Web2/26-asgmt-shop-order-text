# 【課題】注文画面の作成

## 事前準備

1. [こちらのページ](https://classroom.github.com/a/_qqYa4LU)から、ソースコードを`C:¥sys_dev_exe`へcloneする
2. VSCode上で、`Ctrl+Shift+P`(Macの場合は`Cmd+Shift+P`)を押し、コンテナを起動する
3. VSCode上で、`Ctrl+J`(Macの場合は`Cmd+J`)を押し、ターミナルを表示する
4. `composer create-project laravel/laravel .` を実行し、Laravel環境を構築する
5. 過去に作成した以下のコードを、上記「1.」でcloneしたソースコードと同じ場所に上書きする
   
    ```text
    app
    ├── Http
    │   └── Controllers
    │       ├── CartController.php
    │       └── ItemController.php
    ├── Models
    │   ├── Cart.php
    │   └── Item.php
    database
    ├── migrations
    │   ├── 20xx_xx_xx_xxxxxx_create_cart_table.php
    │   └── 20xx_xx_xx_xxxxxx_create_items_table.php
    ├── seeders
    │   ├── DatabaseSeeder.php
    │   └── ItemTableSeeder.php
    │
    途中省略
    │
    public
    ├── css
    │   └── minishop.css
    ├── images
    │   └── xxx.png(15個の画像ファイル)
    │
    途中省略
    │
    resources
    ├── views
    │   ├── cart
    │   │   └── index.blade.php
    │   ├── item
    │   │   ├── index.blade.php
    │   │   └── show.blade.php
    │   └── index.blade.php
    routes
    ├── web.php
    .env
    ```

## 本章の狙い

本章では、今までやったような課題前の練習用の章はございません。
いきなり課題に取り組むことになります。

- 注文画面を再構築する
- アプリケーション「ミニショップ」を完成させる
