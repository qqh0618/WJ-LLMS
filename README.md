# WJ-LLMS
带中文注释讲解的LLAMA3，从零学习大模型

## 安装依赖

## 模型构建步骤

### 构建分词器
   

   **相关关键词：词向量，词嵌入**
   `llms/base/tokenizer.py`


   分词器的作用是将输入的文本转换为模型可以理解的输入向量，同时将模型输出的向量转换为对应的文本。分词器将输入的文本分割成若干个单词，每个单词
   对应一个向量，向量表示单词的含义，然后模型根据向量预测下一个单词，最后将预测的向量转换为对应的单词。
   需要声明的是：分词器是提前训练好的，不能在大模型训练过程中再训练分分词器，训练好的分词器可以理解为键值对。

**比如训练时{"你好":[1,2,3,4]}，那么预测时预测出的向量[1,2,3,4]对应的单词就是"你好"。

但实际分词器的原理和历史发展是很精妙的过程，想详细了解的可以看词向量相关知识。




