# DataDrivenFinance

- 正誤表

| ページ | 誤 | 正 | 
| ---- | ---- | ---- |
|  74  |  $P(\\{X \le -50)$ |  $P(\\{X \le -50\\})$ |
|  74  |  $P(\\{X \le 100)$  |  $P(\\{X \le 100\\})$ |
|  91  |  もし $S_T > K$ であれば  |  もし $S(T) > K$ であれば |
|  91  |  もし $S_T \le K$ であれば  |  もし $S(T) \le K$ であれば |
|  108  |  Johansenのアイデアを紹介したこのアイデアを  |  Johansenのアイデアを紹介した．このアイデアを |
|  184  |  $\mbox{LeakyReLU}(x) = \max(\alpha,x)$  |  $\mbox{LeakyReLU}(x) = \max(\alpha x,x)$ |
|  209  |  もしく次の隠れ層に  |  もしくは次の隠れ層に |

- 追記
  - 9.3.1節 早期終了
    - 例えばp.176のコード例 es = EarlyStopping(monitor = 'loss', patience = 30) のようにオプションで'loss'を指定すると訓練データの誤差が監視対象となる。過学習を防ぐためには'val_loss'が適切。デフォルトでは'val_loss'を指定している。
    - 早期終了を実施する際に最も低いval_lossが得られたモデルを使用する場合は、以下のように'restore_best_weights'オプションを使用する。デフォルトでは'restore_best_weights'はFalseになっている。
      - es = EarlyStopping(monitor='val_loss', patience=30, verbose=1, restore_best_weights=True)
    

  
