# Sentiment_Analysis_of_Citations_using_Sentence_Structure-Based_Features

- 引用の感情分析においてn-gram、科学用語集、依存関係、文の分割など、既存および新規の機能の有効性を調べたもの
- 3-gramとdependecyのパフォーマンスが良い
- positiveとnegativeとobjectiveに分ける

## コーパス
- Bird(2008)によるACL Anthorlogyのデータセットを使用
8736のアノテートされた310論文
- <ICT>というのを付与したため歪んだデータセットとなっている
- そのうち244のpositiveと743のnegativeで残りはobjectiveで歪んだデータセットとなっている
