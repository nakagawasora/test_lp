# 晃商HD 京大生限定長期インターン LP

株式会社晃商HDが実施する、京大生限定長期インターンシップのLPです。

参照サイト: https://www.k-kosho.co.jp/

## 概要

Astroで作成した3ページ構成のランディングページです。
晃商コーポレートサイトの余白感やコピーのトーンを踏襲しつつ、青基調の採用LPとして調整しています。

## ページ構成

| URL | 内容 |
| :-- | :-- |
| `/` | 募集要項、ビジョン、メッセージ、募集フォーム導線 |
| `/departments/` | システム課、広報課、労務課、新規事業立ち上げ予定部署の紹介 |
| `/contact/` | お問い合わせページ。現時点では静的フォームの土台 |

## 再現方法

Node.js 22.12.0以上が必要です。

1. 依存関係をインストールします。

```sh
npm install
```

2. 開発サーバーを起動します。

```sh
npm run dev
```

3. ブラウザで次のURLを開きます。

```text
http://localhost:4321/
```

4. 本番用の静的ファイルを生成する場合は、次を実行します。

```sh
npm run build
```

5. 生成結果をローカルで確認する場合は、次を実行します。

```sh
npm run preview
```

## 主なファイル

```text
/
├── src
│   ├── layouts
│   │   └── Layout.astro       # 共通HTML、ナビ、フッター、共通CSS
│   └── pages
│       ├── index.astro        # 募集要項ページ
│       ├── departments.astro  # 部署紹介ページ
│       └── contact.astro      # お問い合わせページ
└── package.json
```

## 利用コマンド

すべてプロジェクトルートで実行します。

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
