# Sentiment_Analysis_of_Citations_Using_Word2vec
- arXiv(2017)

- タイトル通り，引用感情分析でWord2vecで使用したもの
- sent2vecを使用
sent2vecとは1sentenceのうち，wordそれぞれのベクトルの平均をとったもの

- Training Dataset
ACL Anthology Reference Corpus 
約17000sentences

- Test Dataset
	- ACL Anthology [12]. Athar and Awais [3] (8000引用 830positive, 280negative, 7626objective)
	- 暗黙の物を排除したデータセット
	- positive vs negativeのバイナリ分類

- 結論
word2vecは2項分類(positive vs negativeのバイナリ分類)には有効かもしれない．
ただしn-gramやsentence構造のマニュアルなやり方よりも有効であるとは言えなかった