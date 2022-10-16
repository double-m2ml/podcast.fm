# Episode
- 第48回（2022/10/17）: エンジニアリングの生産性を評価する - GSMフレームワークの紹介
    - リンク: https://anchor.fm/double-m2/episodes/48----GSM-e1pap4h

# Agenda
- 10/8に開催したAWSユーザーグループイベント『JAWS DAYS 2022』の登壇
- エンジニアの生産性を評価するためのGSMフレームワークの紹介

# Contents
## 『JAWS DAYS 2022』の登壇
- 応募人数2,000人超のAWSのユーザーグループイベント
- 発表者はオフライン、参加者はオンラインというハイブリットな構成
- オフラインでの発表環境は快適だった&人前で発表するので、登壇している感があった

## GSMフレームワーク
- エンジニアリングの生産性を計測し、効果を可視化させるためのフレームワーク
    - 書籍『Googleのソフトウェアエンジニアリング』で紹介されている
    - Goal, Signal, Metricで構成されている
        - **Goal**: 望ましい最終結果を表す。特定の方法を参照してはいけない。
        - **Signal**: 最終的な結果を達成したことを知る方法。測定できなくてもよい。
        - **Metric**: Signalの代用品。実際に計測できるものを設定する。
    - 運用方法
        - Goal→Signal→Metricの順番で設定する
        - 計測の前に計測する価値があるかどうかを考える
            - 計測の結果に応じてどのようなアクションを起こすか
            - アクションを誰が, いつ決定するのか



# Reference
- [JAWS DAYS 2022](https://jawsdays2022.jaws-ug.jp/)
- [JAWS DAYS 登壇資料](https://speakerdeck.com/masatakashiwagi/jaws-days-2022-awsnomanezidosabisudeshi-xian-suruniariarutaimunajian-suo-ji-pan)
- [JAWS DAYS 2022で登壇した感想](https://masatakashiwagi.github.io/portfolio/post/my-thoughts-on-speaking-at-jawsdays2022/)
- [Googleのソフトウェアエンジニアリング](https://www.oreilly.co.jp/books/9784873119656/)
- [CI/CD Metrics with GSM Framework](https://engineering.mercari.com/en/blog/entry/20211130-ci-cd-metrics-with-gsm-framework/)
