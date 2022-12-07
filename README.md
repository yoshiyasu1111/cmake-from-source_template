# コンテナのビルド

## 手動でビルドする場合

```bash
$ docker buildx bake -f docker-compose.yml
$ docker compose up -d
```

## vscodeのremote containerでビルドする場合

`Open Folder in Container`でルートディレクトリを開く

# cmakeの利用方法

`cmake -S <ソースディレクトリ> -B <ビルドディレクトリ>`コマンドでプロジェクトのビルドシステムを生成します。

## ビルドシステムの生成

```bash
$ cmake -S . -B build
```

## ビルド

```bash
$ cmake --build build
```
## 実行

```bash
$ ./build/hello 
Hello World!
```
