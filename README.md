# 経歴システム

## システム構成
### プラットフォーム
* AWS EC2(Webサーバー)とRDS(MySql)
* Docker + Linux + MySQL

## 開発手法
* 言語
  * PHP + [Laeavel6](https://laravel.com/)を想定
  * ユーザー認証
    * OAuthを用いた認証(Google等)でアカウントを管理
  
* 開発環境

  * 自PC上にDockerを環境を作成
    * Amazon Linux、Centosイメージを元にする
    
  * 利点
    * 自PCのOSの種類に依存しない
    * Docker Composeを用いる事で、開発環境構築の軽減で、途中参画を容易にする
    
  * 欠点
    * 仮想環境を用いる為、メモリーとディスク容量が、ドキュメント作業中心のPCよりスペックが必要とする

* ドキュメントとソースコードは、GitHub上で管理
  * 利点
    * ドキュメントとコードは誰ても閲覧では、修正を行える
      * [プルリクエスト](https://laraweb.net/environment/1543/)を活用してソースのコンフリクトを防ぐ
    * タスク(Issuesを利用)の可視化
    * 改変履歴の管理    
    * ドキュメントは、テキストベースの[Markdown](https://www.markdown.jp/what-is-markdown/)形式で
      * Gitのブランチを切替えする事で、検証が容易になる
  * 欠点
      * 公開状態なので、社外の方でも閲覧できてしまう
          * 非公開化が必要([無償プランの非公開の制限](https://github.com/pricing))
      * プルリクエストをするには、GitHubにアカウントが必要(閲覧には要らない)
  * 注意点
  
    * 当面は、公開状態で進めるが、最終的には、非公開にする予定    
  * リポジトリ上には、ID、パスワード等の情報は、登録しない
    

## [入力項目](/Doc/input.md)

## [テーブル一覧](/Doc/table.md)

## [検索機能](/Doc/search.md)

## [出力印刷機能](/Doc/print.md)

【補足】

* [今さら聞けない！GitHubの使い方【超初心者向け】](https://techacademy.jp/magazine/6235)
* お勧めMarkdown編集ソフト[Typora](https://typora.io/)
