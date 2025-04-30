
# Structive サンプル集

[English](README.md)


このリポジトリは、**Structive** のサンプルプロジェクトを多数収録しています。各フォルダは独立した実行可能なサンプルであり、テーブル・チャート・ルーターの使い方など、特定のパターンを示しています。

各サンプルは **structive.js** をオープンCDNから直接参照しているため、ビルド工程は不要です。必要なのはモダンなブラウザと、*Live Server* のような簡易的な静的ファイルサーバーだけです。

---

## Structiveとは？

Structiveは**Web Components向けの構造駆動型UIフレームワーク**です。  
命令的なDOM操作や仮想DOMの差分計算の代わりに、以下の特徴を持っています：

- **構造パス**（例：`items.*.name`, `regions.$1.population` など）を一級市民として扱う
- ループ内で **暗黙的なインデックス**（`$1`, `$2`, ...）を使うため、一時変数を宣言する必要がほとんどない
- **getterベースのリアクティビティ** - ユーザーコードではプレーンなESクラスのみ、プロキシは使いません

その結果、HTMLは基礎データ構造とほぼ1対1で対応し、ボイラープレート（定型コード）はほぼゼロに抑えられます。

> **要約** - テンプレートを読めば、状態（state）の形がすぐ分かります。

---

## クイックスタート（Live Server）

### 1．リポジトリをクローン
```bash
$ git clone https://github.com/mogera551/Structive-Example.git
$ cd Structive-Example
```

### 2．*Live Server* をインストール
次のいずれかの方法でインストールできます：

| オプション | インストールコマンド | 備考 |
|------------|---------------------|------|
| **npmパッケージ** | `npm install -g live-server` | 任意のターミナルから利用可能 |
| **VS Code拡張機能** | “Live Server”で検索→*インストール* | HTMLファイルを右クリック→**Open with Live Server** |

### 3．サンプルを起動

#### ターミナル（npmパッケージの場合）
```bash
$ live-server
# LiveServer が http://127.0.0.1:8080（デフォルト）で起動します
```

#### VS Code（拡張機能の場合）
*任意の `index.html` を開き、**Go Live** をクリック（または右クリック→**Open with Live Server**）。*  
ローカルサーバーが起動し、デフォルトブラウザでページが開きます。

---

## リポジトリ構成
```
js-benchmark/        → js-benchmark デモ
radar-chart/         → SVGレーダーチャート（編集可能な統計付き）
states-population/   → 米国州別人口集計
…                    → 今後も追加予定
```
どのフォルダも自由に参照できます。エントリーポイントは常に `index.html` または `*.st.html` で、単体で実行可能です。

---

## コントリビュートについて

新しいサンプルや改善のPull Requestは大歓迎です！  
既存のフォルダ構成に従い、外部アセットは可能な限りCDN経由でお願いします。

---

© 2025 mogera551 · MIT License

Citations:
[1] https://zenn.dev/dai_shi/articles/5ed1b58c5e537a
[2] https://zenn.dev/masaru21/articles/f25393f3ee0813
[3] https://cyber-synapse.com/business-knowledge/marketing/japanese-content-marketing-techniques-in-google/
[4] https://sfia-online.org/ja
[5] https://www.e-sales.jp/eigyo-labo/framework-7331
[6] https://offshore.icd.co.jp/blog/system-development/framework/
[7] https://products.sint.co.jp/topsic/blog/framework
[8] https://www.youtube.com/watch?v=rvX-Xsd5cSc
[9] https://www.bunka.go.jp/seisaku/bunkashingikai/kokugo/nihongo/nihongo_123/pdf/93997901_01.pdf

---
Perplexity の Eliot より: pplx.ai/share