# Formを作る

## 方法
1. Google Forms
   [Google Forms](https://docs.google.com/forms/u/0/?tgif=d)。
   これとHTMLを組み合わせることは無理だった。

2. Google Apps Script にPOSTメソッドで送信
   Google Apps Script で受け取り、スプレッドシートに書き込む。
   デザインも自由。
   セキュリティ面で注意が必要。
   リクエスト送信件数の制限も注意が必要

3. どこかのデータベース(Firebase function)とか
   https://qiita.com/ryo2132/items/7cdd6c86dd418095f74a
   僕はやったことない
   意外と制限ない
   なに使う？


## GETとPOSTの違い
GETは参照に使い、POSTは更新や機密情報で使う。
GETはURLのクエリーでPOSTはボディに含まれたパラメータに格納される。
GETはログにそのまま残るが、POSTは機密情報を守るようにログに残らない。
参考
<https://zenn.dev/ishiyuriniwa/articles/cd24a44933474f>