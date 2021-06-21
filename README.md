# master-nlp1
# 概括
文本分类为自然语言最基础与核心的任务。由于深度学习的出现，上个10年在这方面有大量的研究。文本分类即为文本指定预定义标签是自然语言最核心的任务。
 ## 文本分类应用领域与经典文本分类方法
情感分析、主题标签、问答系统、对话框行为分类等。
![图片](https://user-images.githubusercontent.com/74557964/122555825-5b7f1580-d06d-11eb-98ee-3e51791f9000.png)
Shallow learning model 往往需要通过人工得到好的样本特征并且用经典的机器学习方法进行分类。因此模型的有效性受限于特征提取。与
浅层模型不同的是，深度学习模型通过一系列非线性转换利用模型拟合来替代特征工程，并将特征直接映射到输出的过程。
## 浅层模型分类方法
1960s到2010s主要应用浅层学习模型，具体有：朴素贝叶斯、KNN、SVM等。
与早期基于规则方法相比，优点：有较好的准确率和稳定性，但这些方法需要做特征工程（相当耗时和耗费成本的）另外其也会忽视文本数据的语言结构和上下文信息。因此学习单词的语义信息成为新的热点。
与浅层学习模型相比，深度学习模型可以自动为文本挖掘提供语义信息，以及不需要人工设计规则和处理特征。这些优势决定了大部分学者都是用DNNS来写文献，很少用浅层学习模型来解决有限的计算量和数据。
## 文本分类的发展历程
![图片](https://user-images.githubusercontent.com/74557964/122559183-984d0b80-d071-11eb-8f71-2126e24d18c0.png)
# 文本分类的方法
文本分类其实就是从源数数据中提取特征并利用这些特征来预测文本分类的类别。应用场景主要用：情感分析（SA）、topic labeling(TL)、新闻分类（NC）、问答系统（QA ）、dialog act classification(DAC)、事件预测（EP)等等。
文本分类使用的第一模型是<b>朴素贝叶斯（NB）</b>，涌现了大量通用模型：KNN、SVM and RF等。近年提出的：XGBOOST、LightGBM分类模型。
深度学习模型：TextCNN、大规模文本分类数据集上的有效性为BERT。
## 浅层学习模型
浅层学习模型通过提高准确性来进行文本分类其应用范围更加广泛。第一步为都是为训练模型处理原始文本。具体包括：分词、数据清洗和数据统计。
第二步：文本表示目的就是将文本在信息损失最小的原则下处理成计算机容易利用的信息。具体包括：Bag-of-words（BOW）、N-gram、IF-IDF、woord2vec、GloVe.后续分类的细节描述见其他期刊。
第三步：分类。常用的分类器有：PGM-based models、NB、HMM models、KNN-based methods、SVM-based Methods、决策树算法。Integration-based Methods算法。
总结：缺点：特征工程是一个艰巨的任务，优势：在有限的计算复杂度下，浅层学习模型往往比深层学习模型有更好的效果。
## 深度学习模型
由人工神经网络组成的DNN模型，自动模拟人脑从数据中学习高级特征，与浅层模型相比，在语音识别、文本理解、图形处理等许多领域都获得了更好的效果。
DNN模型的效果可以被下游任务来检验。深度学习进行文本分类任务的前两步都是<b>前馈神经网络和递归神经网络</b>。模型种类：CNN、RNN、attention mechanisms模型融合、多任务方法等。
BERT出现能够产生更符合实际的文本向量是自然语言发展的重要转折点。（技术细节后续补充）ReNN-based Methods、MLP-based Methods。RNN-based Methods。CNN-based Methods。RNN-based Methods。多融合模型。Attention-based Methods。Transform-baser Methods（并行化计算）、GNN-based Methods。
## 数据集和评估指标
![图片](https://user-images.githubusercontent.com/74557964/122725325-7210b100-d2a7-11eb-8a28-705ad60634d4.png)
##  Accuracy rate and Error Rate:
![图片](https://user-images.githubusercontent.com/74557964/122725485-a2584f80-d2a7-11eb-839e-106767f0e411.png)
##  Precision,Recall and F1
![图片](https://user-images.githubusercontent.com/74557964/122725636-c9af1c80-d2a7-11eb-915b-fcd61500b6ec.png)
多任务标签评估指标（暂时性的忽略）
阅读文章启示：综述性文章可以只读大概框架，后续性的技术细节问题，针对框架，慢慢补充与练习，然后回过头来在继续看综述性文章，或许会有更多的启示与收获。






，
