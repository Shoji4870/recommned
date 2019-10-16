# recommneder system
- Jester Datasetを使ってユーザにジョークをお薦めするシステムを実装
- 今回実装したレコメンド手法
    1. コンテンツベースフィルタリング
        - ジョークをベクトル化するのには，TF-IDFを使用
        - LSA(Latent Semantic Analysis)を使って，ジョーク間の類似度を算出
            - SVD(sigular value decomposition)
            - これの精度が上がらなかったので，TF-IDFを使用する前にジョークをステミング
    2. 協調フィルタリング
        - ユーザベース
        - 標準化（中央化）
