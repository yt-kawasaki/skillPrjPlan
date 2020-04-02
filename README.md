# 経歴システム
[toc]
## システム構成
### プラットフォーム
* AWS?
* Docker + Linux + MySQL

## 開発方法
* 言語
  * PHP + Laeavel6
  * ユーザー認証
    * OAuthを用いた認証(Google等)
* 自PC上にDockerを環境を作成
  * Amazon Linux、Centosイメージを用いる
  * Docker Composeを用いて、環境構築する
* ドキュメントとソースコードは、Github上で管理
  * 目的
    * コードとドキュメントをオープンにしてシステム化する
    * タスクの管理(Issuesを利用)
  * 当面は、公開状態で進めるが、最終的には、非公開にする
  * 注意点
    * ID、パスワード等の情報は、登録しない
* 本番環境は、Githubからのコードからリリースする
