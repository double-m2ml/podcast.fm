# Episode
- 第46回（2022/09/26）: 今話題のStable Diffusionについて
    - リンク: 

# Agenda
- Stable Diffusionの話題性
- Stable Diffusionの概要
    - Diffusion Model（拡散モデル）
    - CLIP
    - モデルネットワーク構造
    - Dataset
- Stable Diffusionの商業利用について

# Contents
- Stable DiffusionはSNSで盛り上がっている
    - オープンソース化＆demoなどが公開されており誰でも試せる
- Diffusion Model
    - 画像生成モデルの主流
    - ノイズを除去して画像を生成する
    - CNNベースのモデルとは異なるアプローチ
    - 計算量が多く、学習だけでなく推論にも時間がかかる
- CLIP (Contrastive Language-Image Pre-training)
    - 画像とテキストとの関連性を学習したモデル
    - Stable Diffusionではユーザーが入力したテキストを処理するために使用される
- 巨大なデータセット
    - Stable Diffusionモデルの学習には[LAION-5B](https://laion.ai/blog/laion-5b/)という58億件のデータセットが使われている
- Stable Diffusionの商業利用
    - Figmaのプラグインによる製品デザイン
    - 著作権の問題
        - 技術の発展を妨げず、表現者に不利にならないような落としどころを考えていく必要がある

# Reference
- [Stable Diffusion with Diffusers](https://huggingface.co/blog/stable_diffusion)
- [2022年度・深層学習による写実的画像合成の最新動向](https://speakerdeck.com/ykanamori/2022nian-ban-shen-ceng-xue-xi-niyoruxie-shi-de-hua-xiang-he-cheng-nozui-xin-dong-xiang)