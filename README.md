# ポートフォリオ

## 買い物アプリ

Railsで作った簡単なECサイトです。

### 実物(AWS)(停止中)

http://ec2-176-34-29-202.ap-northeast-1.compute.amazonaws.com/

### ソースコード

https://github.com/youmts/sample-market

- rails 5.2.4.3
- ec2 + rds
- ちょっとややこしめの[モデル実装](https://github.com/youmts/sample-market/blob/master/app/models/order.rb)
- CircleCIで[rspecチェック](https://github.com/youmts/sample-market/blob/master/.circleci/config.yml)
- google-oauth2

## Atcoder 解答集

プログラミングコンテストAtcoderの解答集です。

### ソースコード

https://github.com/youmts/atcoder

- [abc118/d.rb](https://github.com/youmts/atcoder/blob/master/abc118/d.rb) のように一回層下に解答のソースを配置（すべてruby,アルファベット順に難易度が上がる）
- ソースの先頭に問題文へのリンクあり
- 8回参加してレート1052 https://atcoder.jp/users/youmts
- プログラミングコンテストなので可読性は良くない

## 都道府県別総人口のチャート表示

フロントエンド(Vue.js)の勉強で作ったものです。

### 画面イメージ

<img src="https://user-images.githubusercontent.com/8408731/88469003-b2946d00-cf26-11ea-90c3-ab06f4961045.gif" width="400">

### 実物(heroku)

https://thawing-hollows-68596.herokuapp.com/

### ソースコード

https://github.com/youmts/resas-chart

- こちらのAPIを利用： https://opendata.resas-portal.go.jp/
- rails + Vue.js + chart.js
- クライアントだけでやろうと思ったが、APIキーをクライアントに載せたくなかったので、データ中継用にrailsを
- vue部分の制作時間３-４時間 : - [ChartContainer.vue](https://github.com/youmts/resas-chart/blob/master/app/javascript/containers/ChartContainer.vue),[PrefecturePopulationChart.js](https://github.com/youmts/resas-chart/blob/master/app/javascript/components/PrefecturePopulationChart.js)

## クレジットカード入力フォーム

[フロントエンドのコーディング課題](https://qiita.com/baby-degu/items/d68e52a0727248ba2750)から、フロントエンド(Vue.js)の勉強のためにつくってみました。

### 画面イメージ

<img src="https://user-images.githubusercontent.com/8408731/88344054-c3ee4580-cd7d-11ea-87ce-188270da567e.gif" width="400">

### 実物（S3)(停止中)

http://demo-credit-card-form.s3-website-ap-northeast-1.amazonaws.com/

### ソースコード

https://github.com/youmts/credit-card-form

- お手本： https://github.com/muhammederdem/vue-interactive-paycard
- Vue.js + typescript
- github actions を使って s3 にデプロイ
- Vuelidate でバリデーション
- カードをひっくり返すところはできていない
- vue部分の制作時間5-6時間 : [containers](https://github.com/youmts/credit-card-form/tree/master/src/containers), [components](https://github.com/youmts/credit-card-form/tree/master/src/components)
