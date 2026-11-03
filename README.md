# ミニゲーム集

スマホで遊べる、1ファイル完結（HTML + CSS + JS 同梱、ビルド不要）のミニゲームを集めたリポジトリ。

公開URL: https://hrk-mrks.github.io/claude-sandbox/

## ディレクトリ構成

```
.
├── index.html              # トップページ（ゲーム一覧）
├── games/
│   ├── sushida/
│   │   └── index.html      # 🍣 スマホ寿司打
│   ├── gacha/
│   │   └── index.html      # 💎 無限ガチャ
│   ├── platformer/
│   │   └── index.html      # 🍄 ジャンプアドベンチャー
│   └── tetris/
│       └── index.html      # 🧱 テトリス
├── README.md
└── .github/workflows/pages.yml   # main への push で GitHub Pages に自動デプロイ
```

## ゲーム一覧

| ゲーム | パス | 概要 |
| --- | --- | --- |
| 🍣 スマホ寿司打 | `games/sushida/` | 60秒ローマ字タイピング。shi/si など入力ゆれ対応 |
| 💎 無限ガチャ | `games/gacha/` | 石1000個（単発10・10連100で11体）。★3〜★6のモンスター、レア度別演出、使い切ると集計表示 |
| 🍄 ジャンプアドベンチャー | `games/platformer/` | 横スクロールアクション。ステージ選択（★1〜★3）、タッチ操作、敵踏み・コイン・?ブロック・動く足場・チェックポイント、ベストタイム保存 |
| 🧱 テトリス | `games/tetris/` | タップで回転・長押しで高速落下・横ドラッグで移動・下フリックでハードドロップ。ゴースト表示、NEXT、レベル制、ベストスコア保存 |

## ゲームを追加する

1. `games/<ゲーム名>/index.html` を作る（1ファイルで完結させる）
2. ルートの `index.html` の一覧にカードを1つ追加する
3. この README のゲーム一覧に1行追加する
4. `main` に push すると自動でデプロイされる

## ローカルで試す

```sh
python3 -m http.server 8000
# http://localhost:8000 を開く
```
