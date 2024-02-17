# 📚 Chinese Historical Documents Assistant(CHDA)

## 中国历史文献推荐小助手

基于 `DGL（Deep Graph Library）` 框架训练模型，内置了自采数据集、训练过程、评测过程以及一个小应用。

## 快速开始

`pip install dgl torch` 或参考：[https://www.dgl.ai/pages/start.html](https://www.dgl.ai/pages/start.html)

`pip install gensim fasttext`

## 数据集

自行导出到 `paper.json`，目前提供一个简单的数据集

## 主函数

目前仅提供了一个非常基础的文本特征处理方式（简单的词袋模型），在实际应用中，您可能需要使用更高级的文本表示方法，如 TF-IDF、Word2Vec 或 BERT 等。
此外，超边到图的转换过程也需要根据您具体的数据结构和需求来设计。

## 训练与验证

```python
WIP
```

## 小应用

`WIP`

## Roadmap

- [ ] 文本特征的预处理：对于文本类特征（如标题和摘要），通常需要通过自然语言处理技术将其转换为数值型特征向量，常用的方法包括 TF-IDF、Word2Vec、BERT 等。
- [ ] 特征工程：对于类别型特征（如作者），可以使用独热编码(one-hot)等技术。此外，还可以设计特定的特征，如基于引用数量的特征，来捕捉节点的影响力等属性。
- [ ] 模型设计：设计图神经网络模型时，需要考虑如何有效整合节点特征和图结构信息。这可能涉及选择合适的图卷积层、激活函数、以及正则化技术等。
