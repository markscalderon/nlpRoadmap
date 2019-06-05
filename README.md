# nlpRoadmap

## Reference
[GitHub - DeepNLP-models-Pytorch](https://github.com/huankiki/DeepNLP-models-Pytorch)  
[GitHub - nlp-tutorial](https://github.com/huankiki/nlp-tutorial)  
[GitHub - nlp-roadmap](https://github.com/HaveTwoBrush/nlp-roadmap)  


## Theory, 理论篇： Deep Learning
- [x] RNN
- [x] LSTM/GRU
- [x] TextCNN


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
[fastText论文解读、fastText与word2vec的区别和联系](https://blog.csdn.net/u011239443/article/details/80076720)  
  - fastText可以用来学习词向量，也可以进行有监督的学习，如文本分类
  - 相似点：fastText的结构与word2vec的CBOW的结构相似，并且采用了相同的优化方法，如Hierarchical Softmax
  - 不同点：有监督fastText其实是将CBOW模型的中心词改成label（即输出层变化），将上下文词改成整个句子中的词，包括N-gram（即输入层变化）
  
### Pretrained NLP Models
[从Attention,Transformer,ELMO,GPT到BERT](http://www.bdpt.net/cn/2019/01/22/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%EF%BC%9A%E5%89%8D%E6%B2%BF%E6%8A%80%E6%9C%AF-%E4%BB%8Eattentiontransformerelmogpt%E5%88%B0bert/)  

- [x] Seq2Seq  
真正提出Seq2Seq的是文献[1]，但文献[2]更早地使用了Seq2Seq模型来解决机器翻译的问题。文献[1]引用了文献[2]。
  - [1] Sequence to Sequence Learning, 2014, Google  
 此文的工程性更强，计算量很大：8-GPU machine, Training took about a ten days with this implementation
  - [2] Learning Phrase Representations using RNN Encoder–Decoder for Statistical Machine Translation, 2014  
  文献[2]末尾详细给出了**RNN Encoder-Decoder**的公式推导，此文的**最大贡献是提出了GRU结构**，LSTM的简化版。
- [x] Attention  
此文作者与Seq2Seq的作者相同，包括Yoshua Bengio大神，学术味很浓，公式推导很详尽。  
此文是第一个将attention机制应用到NLP领域的工作，把attention机制用到了神经网络机器翻译的RNN Encoder-Decoder模型中。  
[Attention论文的中文翻译](https://blog.csdn.net/qq_20135597/article/details/83758013)  
延伸阅读：[注意力机制（Attention Mechanism）在自然语言处理中的应用](https://www.cnblogs.com/robert-dlut/p/5952032.html)  
![](./graph/attention_example.png)  
- [x] **Transformer**  
从英语阅读来讲，此文易读，但是看不懂:(  
拜读了对Transform的解读之后，感慨：Transform真的是简约不简单！ 推荐：  
[The Illustrated Transformer-Jay Alammar](https://jalammar.github.io/illustrated-transformer/)  
[The Illustrated Transformer【译】](https://blog.csdn.net/yujianmin1990/article/details/85221271)  
- [ ] ELMO
- [ ] OpenAI GPT
- [ ] Google BERT  
与Transform的那篇解读是同一个Blog。  
[The Illustrated BERT, ELMo, and co. (How NLP Cracked Transfer Learning)-Jay Alammar](https://jalammar.github.io/illustrated-bert/)  
[The Illustrated BERT【译】](https://blog.csdn.net/qq_41664845/article/details/84787969)


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

