# Application of Universal Sentence Encoder

TensorFlow hubで公開されているUniversal Sentence Encoderを用いて、

- [文間類似度の計算](https://github.com/marucha80t/application_of_universal_sentence_encoder/blob/master/sentence_similarity.ipynb)
- [教師なし抽出型要約](https://github.com/marucha80t/application_of_universal_sentence_encoder/blob/master/unsupervised_extractive_summarization.ipynb)

を行う。



## 文間類似度の計算

Universal Sentence Encoderは日本語以外にも、英語・ドイツ語・フランス語など複数の言語に対応している。ここでは、日本語文同士の文間類似度に加えて、その日本語文を英文に翻訳した文との類似度も算出し、ヒートマップに示す。



## 教師なし抽出型要約

Universal Sentence Encoderを用いて、入力文書及びその文書中に含まれる各文をそれぞれベクトル化する。

各文をEmbedRank++を用いてランキングし、上位n件を要約文として抽出する。



## 参考

- [TensorFlow Hub: universal-sentence-encoder-multilingual](https://tfhub.dev/google/universal-sentence-encoder-multilingual/1)
- [Simple Unsupervised Keyphrase Extraction using Sentence Embeddings](https://arxiv.org/abs/1801.04470)
