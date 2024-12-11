## プロジェクト概要

まだ進行中の個人作成アプリです。
ユーザーがローカルから英語内容の個人PDFファイルをアプリに読み込み、単語分割、翻訳、読み上げできるようにしています。
将来的にはメイン機能が影響を受けない前提でPDFファイルでの読み物提供の代替案を実装する予定です。
単語の記憶ステータス管理ができます。（例：本を読む途中、その後）

まだ開発中と将来的にストアにリリースの為ソースコードの公開はありません。


## 主な機能

- [ユーザーの書籍登録]
- [書籍内容の閲覧時の単語分割]
- [単語の記憶ステータス管理]
- [翻訳、読み上げ]

## スクリーンショット

| ![Image 1](./1.png) | ![Image 2](./2.png) | ![Image 3](./3.png) |
|---------------------------------|---------------------------------|---------------------------------|
| ![Image 4](./4.png) | ![Image 5](./5.png) | ![Image 6](./6.png) |



## 技術スタック
- SwiftUI
- SwiftData
- Observation
- NaturalLanguage
- PDFKit
- AVKit（読み上げ用）

## 開発上の課題と解決策

- PDFファイルの１ページずつの内容から句に分割していますがページによってそのページで句が終わらない場合はがあり、解決案はありますが、実装していません。
- デザインに関して色々変えてみたりしましたが変動頻度が高いので現時点ではあまりには気に入らないままのUIになっています。
- PDFファイルをアプリに読み込みの代替案には一人として作業量がありそうです。


## 追記
PDFのやり方は基本ユーザ任意でコンテンツをアプリに入れて使うのですが、やはり著作権の問題、登録の不便性などの為名言の引用（Quote）などから学習内容を選べるような仕組みを作るREST API：
https://github.com/KaneEast/english-app-api
を開発してiOSアプリ側で使えうるように工夫しています。
https://github.com/KaneEast/english-app-api

| ![Image 7](./7.png) | ![Image 8](./8.png) | ![Image 9](./9.png) |
