# Mermaid Viewer

Mermaid 記法をブラウザ上で素早くプレビューできる、シンプルな静的 Web ツールです。  
テキストエリアに記法を書いて **描画** ボタン（または `Ctrl/Cmd + Enter`）を押すと、右側に SVG 図を表示します。

## 主な機能

- Mermaid コードのリアルタイム描画
- `Ctrl/Cmd + Enter` ショートカットで描画
- Mermaid コードのクリップボードコピー
- エディタ内容のクリア
- `sessionStorage` で直前に描画したコードを保持
- `click ノードID callback "説明文"` 形式に対応（ノードクリック時に説明表示）

## 使い方

1. Mermaid 記法を左側のエディタに入力します。  
2. **描画** を押すか、`Ctrl/Cmd + Enter` を実行します。  
3. 右側のプレビューに図が表示されます。  
4. 必要に応じて **コードをコピー** / **クリア** を利用します。

## ローカルで起動する

このプロジェクトはビルド不要の静的サイトです。`docs/index.html` を配信できれば動作します。

### 例: Python でローカルサーバーを起動

```bash
cd docs
python3 -m http.server 8000
```

ブラウザで `http://localhost:8000` を開いてください。

## ディレクトリ構成

```text
.
├── README.md
└── docs/
    ├── index.html      # アプリ本体
    ├── favicon.ico
    ├── chroco_icon.png
    └── CNAME
```

## 利用技術

- [Mermaid](https://mermaid.js.org/)
- [Tailwind CSS (CDN)](https://tailwindcss.com/)

## ライセンス

必要に応じて、プロジェクト運用方針に合わせて追記してください。
