# Laravel Sail確認用プロジェクト

Laravel Sail環境を確認するためのプロジェクトです。
独自のDocker Compose環境を作っていくため、詰んだ場合に参考にする。

前提として、WSLにcomposerをインストールしている必要があります。
asdfでphpをインストールした際にcomposerをインストール済み。

# Laravel 10 プロジェクト作成

```sh
# curl -s https://laravel.build/src | bash
mkdir v10
cd v10
composer create-project "laravel/laravel=10.*" ./
php artisan sail:install
# インストール中にmysql、redisなどのサービスを選択できる
```

