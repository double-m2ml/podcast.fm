# Episode
- 第40回（2022/07/18）: 記事紹介 - Trustworthy AI is Built on Trustworthy Data
    - リンク: https://anchor.fm/double-m2/episodes/--Trustworthy-AI-is-Built-on-Trustworthy-Data-e1l9r40

# Agenda
- データの品質に関係する記事『Trustworthy AI is Built on Trustworthy Data』の紹介と品質に対する取り組みについて2人で議論しました
- 下記Referenceに記事のリンク先があります

# Contents
- 海外記事『Trustworthy AI is Built on Trustworthy Data』の紹介
    - MLをビジネスに適用して成功するためには，Trustworthyなデータが必要不可欠である
    - Trustworthyなデータに関して4つの章でまとめられている

## 1. **What is data quality?**
- データの品質を測るための5つの要素
    - **Completeness**： データの完全性
    - **Reliability**： データの信頼性
    - **Accuracy**： データの正確性
    - **Consistency**： データの一貫性
    - **Timeliness**： データの適時性
- データの品質をどのように測るかという問いに対して詳細に説明がされている
- データの適時性について
    - asteriamさんはあまり意識していなかった
    - データ更新の重要性（最新のトレンドを反映しているのか、など）
    - リアルタイムやイベントをトリガーとする処理（データの整合性を担保する）が難しい
    - モデルの用途に応じたデータの更新頻度を考える必要があるのでは

## 2. **What are the potential limitations of the data and how do we measure them?**
- データセットの品質を定義するためにメトリックやスコアをきちんと定義する必要がある
- 品質を評価する指標の例
    - 属性やカラムの欠損
    - レコードの重複数
    - 書式の一貫性（日付など）
- やらなくても最悪モデルを作れてしまうので、優先度が上がりにくい
    - データ基盤で管理する仕組みが重要
- 指標を確認したうえで品質がどうだったかを評価するのは難しい印象
    - 指標を確認したからと言ってデータセットの品質の良し悪しを評価する判断するためにはもう一段階の考察が必要
    - 欠損や重複が多いとモデルにどう影響を及ぼすかを考える必要はある（精度との相関など）

## 3. **How to ensure the gaps do not arise further?**
- Sensitize consumers and producers of your data to known issues:
    - データはアナリストやサイエンティスト以外も扱うことがある。データの品質はモデルに影響を及ぼすため再学習の実行を検討することに繋がる。
- Collaboration is key:
    - データの内容や生成に関する情報（属性やスキーマ、データ型など）を共有しドキュメント化する
    - データを作る側と使う側は異なることが多く、作る側の情報はあまり共有されていない
        - データの生成や性質に何かしらの前提条件がある場合、それを知らないまま分析をしてしまうと、アウトプットの質が低下してしまう
        - 日々使う側と作る側の情報共有やドキュメント化は非常に重要
    - データに関係するエンジニアはビジネスサイドなどとコミュニケーションする頻度が高い傾向にある
        - 機械学習のタスクを考えるうえで、ビジネスサイドとコミュニケーションする必要はあるものの、なかなかそこまでできている人は少ない印象
        - モデルを作るのではなく、そもそもどういうデータを取ってきて、どのような課題に落とし込めるかを考えられる人の需要は高い

## 4. **Have you identified all gaps or is there more to it?**
- 継続的な取り組み（イテレーション）とモデルの定期的な監視は大切
    - 一回モデルを作って終わり、ではなくメトリクスを監視し、定期的な再学習は必要
- 定期的な再学習ができる仕組みとともに、どのメトリクスを監視するのか、いかにビジネスメトリクスに紐づけるかが大事になっている印象
    - データのドリフトの発生検知や分析ができる仕組みを整えていく必要がある
- オペレーションに正解はない
    - MLがビジネスに価値を出すために、何を目的にするのかという意識を持つことが重要
    - モデルの性能とビジネスメトリクスを紐づける、モニタリングすることが大事
    - 性能が劣化した際にデータの異常をフィードバックできる仕組みや体制が望まれる

# Reference
- [Trustworthy AI is Built on Trustworthy Data](https://heartbeat.comet.ml/trustworthy-ai-is-built-on-trustworthy-data-1584b795fbd5)
