# Episode

- 第30回（2022/02/14）: 人工生命やゲームを題材としたAIの技術検証
  - リンク: https://anchor.fm/double-m2/episodes/30-AI-e1eau22

# Agenda

- ゲームに関連したAIの活用事例や面白い記事を紹介

# Contents

### asteriam

- **マリオカート64の自動走行**
  - [記事リンク](https://gigazine.net/news/20211125-mario-kart-64-self-driving/)
    - Nintendo64の実機からプレイ画像を取り込み学習
    - ラズパイによりコントローラーを制御する
    - 現実世界で行われている自動運転と近しい構成
    - モデルはシンプルなCNNで構成されている
    - ゲーム画面にあるタイムやマップを除外するとパフォーマンスが向上した
    - 別のコースで追加学習をすると、わずか2ラウンドで走破できた
    - AIになじみがない人でもわかりやすい例

- **マインクラフト - Kubernetes互換の管理ツール**
  - [記事リンク](https://gigazine.net/news/20220107-kubecraftadmin/)
    - マインクラフトを互換ツールに仕立て上げた
    - マインクラフト上の各種オブジェクトとKubernetesの構成群と対応
    - 例として、Podとブタを連携すると
      - Podの構成数を増やすと、ブタが増える
      - マインクラフト上でブタをKillすると、Podが落ちる
    - Kubernetesの環境をマインクラフト上で可視化できるという面白い仕組み
    - マインクラフトは強化学習の実験の場として最適なのでは？

### navi

- **ARTILIFE**
  - [記事リンク](https://www.itmedia.co.jp/news/articles/1905/17/news060.html)
    - ドワンゴが開発した人工生命をテーマとしたゲーム（2019年6月サービス終了）
    - AIの一つの研究対象である人工生命を観察、飼育するゲーム
    - 餌をあげたり周囲の環境、他の人工生命との相互関係性に応じて行動が変わる（性格）
    - 生命とは何か、人間とは何かといった深遠なテーマを考えさせられる
    - 「生命に対する侮辱」といった否定的なコメントもあり、AIの倫理性に通じる観点もある
- **ボイドモデル**
  - [記事リンク](https://www.bioerrorlog.work/entry/boids-flocking-godot)
    - 鳥の群れをシミュレーションした数理モデル
    - アルゴリズムで生物の動きを規定する人工生命の有名な事例
    - 分離，整列，結合の3つの力を指定することで、群れの動きを再現できる
    - 複数の鳥の相互関係で複雑な動きを表現ができる（物理における複雑系）

# Reference

- [AIを用いたマリオカート64の全自動走行がNINTENDO64の実機で成功](https://gigazine.net/news/20211125-mario-kart-64-self-driving/)
- [「人類には早すぎた」　人工生命観察プロジェクト「ARTILIFE」が私たちに問いかけるもの](https://www.itmedia.co.jp/news/articles/1905/17/news060.html)
- [マインクラフトをKubernetes互換の管理ツールにしてしまった人物が出現](https://gigazine.net/news/20220107-kubecraftadmin/)
- [Godot EngineでBoids Flockingシミュレーションを実装する | 人工生命](https://www.bioerrorlog.work/entry/boids-flocking-godot)
