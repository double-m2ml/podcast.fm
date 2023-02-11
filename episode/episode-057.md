# Episode
- 第56回（2023/02/13）: 2022年おすすめのPythonライブラリ10選の紹介
    - リンク: 

# Agenda
- "Top Python libraries of 2022"という海外記事の紹介
    - 2015年から実施しており今回で8回目
    - AIやデータサイエンスの領域に強く影響された選出になっている（もちろんnon-data science目的のものもある）
- 二人の興味がある or おすすめは...本編でも気になったポイントを紹介してます！
    - asteriam: **Mito**
    - navi: **Diffusers**

# Contents
1. Ruff - a fast linter
    - Pythonでよく使われているリンターを高速化したもの（従来のpylintなどと比較して10~100倍速い）
2. Python-benedict - a dict on steroids
    - build-in dict（辞書のネスト？）の扱いが簡単になる
3. Memray - a memory profiler
    - メモリのモニタリングで，デバッグにも便利
4. Codon - a Python compiler using LLVM
    - Pythonの高速化のためのコンパイラで，従来の10~100倍の速度改善
5. LanfChain - building LLM - powered apps
    - LLM: large language models (GPT-3, ChatGPTなど)
    - LLMを効率よく使うためのインターフェースを提供
    - プロンプト管理：入力のテキスト（プロンプト）と出力結果
6. fugue - distributed computing done easy
    - 分散処理を使いやすくするライブラリ
7. Diffusers - generative AI
    - Diffusion modelsを使うためのインターフェースになるライブラリ
    - Stable Diffusionなど
8. LineaPy - convert notebooks to production pipelines
    - prod環境でJupyter Notebookを使うためのモノ
    - data pipeline (Airflow, Prefectなど)や再現性の確保など
9. whylogs - model monitoring
    - モデルモニタリングのオープンソースライブラリ
    - データセットのサマリなどモデルのインプットになるプロファイルを生成できる
10. Mito - spreadsheet inside notebboks
    - jupyter notebook上でcsvなどExcelっぽく操作できる
    - pythonコードも生成してくれる

# Reference
- [Top Python libraries of 2022](https://tryolabs.com/blog/2022/12/26/top-python-libraries-2022)
