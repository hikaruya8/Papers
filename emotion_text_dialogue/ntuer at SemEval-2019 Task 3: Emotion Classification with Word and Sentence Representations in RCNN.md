# ntuer at SemEval-2019 Task 3: Emotion Classification with Word and Sentence Representations in RCNN

## Peixiang Zhong, Chunyan Miao (2019)

### 要約
EmotionLineデータセットを利用した感情検出タスク
3つの発話を一つの文章にconcatしてembedding layerに入れた。論文内ではこれが文脈情報を加味していると主張している。
ちなみに流行りのELMoやBERTなどの一般化された単語表現は役に立たなかったらしい。
最終的なF値は
DeepMoji + InferSent (fastText)で0.7344


### Embedding
- pre-trained word representaion
fine-tuned the word embeddings obtained from (Baziotis et al., 2017), which has a size of 100 and is pre-trained on 330M English Twitter mes- sages using Glove (Pennington et al., 2014).

- pre-trained sentence representation
DeepMoji(Felbo et al., 2017) 

### 提案モデル(RCNNモデル)
主な構成
- BiLSTM
- linear transformation layer
- max-pooling layer
![figure005](../image/005.png)
