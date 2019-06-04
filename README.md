# nlpRoadmap

## Reference
[GitHub - DeepNLP-models-Pytorch](https://github.com/huankiki/DeepNLP-models-Pytorch)  
[GitHub - nlp-tutorial](https://github.com/huankiki/nlp-tutorial)  
[GitHub - nlp-roadmap](https://github.com/HaveTwoBrush/nlp-roadmap)  

## Theory, 理论篇： Language Model & Word Embedding
### Word Embedding
- [x] NNLM
- [x] word2vec
  - [x] Skip-gram
  - [x] C-BOW
- [x] GloVe  
[GloVe词向量理解](https://www.jianshu.com/p/5bbb55c35961)  
[GloVe与word2vec的联系](https://ranmaosong.github.io/2018/11/21/nlp-glove/)  
***GloVe可以被看成是更换了目标函数和权重函数的全局word2vec***  
- [x] fastText

### Pretrained NLP Models
[从Attention,Transformer,ELMO,GPT到BERT](http://www.bdpt.net/cn/2019/01/22/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%EF%BC%9A%E5%89%8D%E6%B2%BF%E6%8A%80%E6%9C%AF-%E4%BB%8Eattentiontransformerelmogpt%E5%88%B0bert/)
- [ ] Attention
  - [ ] Seq2Seq
- [ ] Transformer
- [ ] ELMO
- [ ] OpenAI GPT
- [ ] Google BERT

## Theory，理论篇： Deep Learning
- [x] RNN
- [x] LSTM/GRU
- [x] TextCNN

## Practice，实践篇
[FudanNLP/nlp-beginner](https://github.com/FudanNLP/nlp-beginner)

### Sequence Labelling, POS Tagging/NER
序列标注：词性标注/命名实体识别
- [ ] HMM
- [ ] CRF
- [ ] MEM，最大熵
- [ ] (Bi)LSTM + CRF

### Text Classification & Sentiment Analysis
文本分类、情感分析
- [ ] LR/Softmax + BOW/tf-idf + n-gram
- [ ] SVM + BOW/tf-idf + n-gram
- [ ] TextCNN
- [ ] LSTM + Word Embedding

### Language Model (NN)
基于神经网络的语言模型的训练
- [ ] word2vec/gensim
- [ ] RNN/LSTM/GRU

### Dialog System
对话系统

### Topic Model
主题模型
- [ ] LDA

