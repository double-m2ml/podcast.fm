# Episode
- 第14回（2021/09/20）: 第1回-技術書紹介
    - リンク:　https://anchor.fm/double-m2/episodes/14-1---e17hb87

# Contents
- 最近読んだ/読んでる技術書紹介

## 内容
- 最近読んだ/読んでる技術書についてお話しました
  - asteriam
    - 実務でも取り組んでいるレコメンドシステムに関する書籍を紹介
    - 特にレコメンドシステム評価について気になっているので，そこを調べてます
      - オフライン・オンライン評価
        - 予測指標やランキング指標，A/Bテストなど
    - どういった場面でどのような評価を行えば結果を正しく判断できるのか，タスクに応じてどういった評価指標を用いれば良いのかなどを調べたりしています
        
  - navi
    - 仕事ではじめる機械学習という書籍を紹介
    - その名の通り仕事で機械学習をはじめるにはうってつけの本
    - 機械学習の基礎はあらかじめ知っていること前提
    - 機械学習を実装できるけど，ビジネスに転換させるためにはどうするか，というのを紹介している
    - 本を読む前はモデル実装できます人間だったけど，ビジネスに使うためにはモデルを安定的に運用したり，モニタリングしたりということの重要さを知った
    - 転職したことで↑について結構気付かされたけど、本を読むことで改めて確認
      - 例えば，モデルの学習と推論の周期によってシステムは大きく変わる
				学習と推論をそれぞれバッチ処理するのか，リアルタイム処理をするのかなど
      - 学習，推論処理を簡便にするためのパイプライン設計
        - AirflowやKubeflowなど
      - 前処理の共通化を目的としたFeature Storeの導入
    - 他にも効果検証の話やブラックボックスなモデルの解釈方法，バンディットモデル（強化学習），オンライン広告をテーマにした機械学習を用いた意思決定デザインなども紹介

## Reference
- [推薦システム-統計的機械学習の理論と実践-](https://www.kyoritsu-pub.co.jp/bookdetail/9784320124301)
- [Evaluating Recommendation Systems](https://link.springer.com/chapter/10.1007/978-0-387-85820-3_8)
- [仕事ではじめる機械学習 第2版](https://www.oreilly.co.jp/books/9784873119472/)