# Episode
- 第18回（2021/10/25）: Personality Bias of Music Recommendation Algorithmsという論文の紹介
    - リンク: https://anchor.fm/double-m2/episodes/18-Personality-Bias-of-Music-Recommendation-Algorithms-e197hub

# Agenda
- 音楽におけるPersonality特性の違いによるレコメンドアルゴリズムのバイアスに関する論文

# Contents
- 性別，年齢，国，消費行動などが異なるグループにおいて，レコメンドシステムのパフォーマンスが異なることが知られているが，本論文では，このユーザーのバイアスをユーザーのpersonality（性格）という観点から調査をしている
- Twitterユーザーの音楽消費行動とPersonality特性のデータセットを作成して，OCEANモデルの観点から特性を調査している
- 論文の結果から以下のことが言える
    - Personality特性のスコアが低いと ，開放性・外向性・誠実性のパフォーマンスが高くなり，神経症と協調性のパフォーマンスが低くなる
    - 性格が異なるユーザーに対して，神経症と開放性で非常に有意な差が見られた（Recall/NDCG共に）
- 論文を読もうとしたきっかけは？
    - パーソナリティがキーワードとして気になる（1to1のレコメンド）
    - 今まで漠然としていたけど，どういうパーソナリティがあるのか，定量的な結果が出ていることで考えが広がった
- 性格にレコメンドのバイアスがある場合は，将来的にレコメンドエンジンを作るにあたり変えていくべきことはあるのか？
    - 事前に心理テスト的なものをして，それも説明変数に入れ込むとか？
    - レコメンド指標としての多様性やセレンディピティの評価も取り入れることでバイアスを緩和できるのではないか
    - アルゴリズムの結果がよくないもの（興味がなさそうなもの）もリストに取り込む（ランダム性を持たせる）

# Reference
- [Personality Bias of Music Recommendation Algorithms](https://dbis.uibk.ac.at/sites/default/files/2021-05/manuscript.pdf)
- [The Big Five Personality Traits](https://www.verywellmind.com/the-big-five-personality-dimensions-2795422)
