# ML_Class6
## Models on the Sesame Street
## Introduction of Bert
### Self-supervised Learning
1. Supervised: 有label才能訓練supervised model
   Self-supervised: 在沒有label的情況下自己做supervise
2. Masking: BERT在訓練的時候，輸入一個具自，先隨機決定哪些中文字要被蓋起來，再決定要如何蓋住(有兩種方法：把某個字換成某特殊符號代表蓋住or把某個字換成另一個字)
3. Next Sentence Prediction： 預測某兩個句子是否為相接的，但這個任務對Bert的訓練沒有幫助 -> Sentence order prediction對Bert是有用的
### How to use BERT?
1. BERT(self-supervised learning)算是un-supervised(在學填空題的階段)也算是semi-supervised(因用在下游任務時，需要有少量標註的資料)
   BERT PRE-TRAINED + FINE-TUNED -> semi-supervised
## Fun Facts about BERT
### How does BERT work?

## GPT-3
### GPT要預測接下來會出現的token是什麼
1. GPT的想法跟BERT不一樣，因為GPT的模型太大了，大到連fine-tune都有困難！
   
   GPT的使用方式：few-shot learning without gradient descent（in-context learning），只給他一些例子讓他去學習

## Auto-Encoders: Basic Concepts
1. Auto-Encoder算是self-supervised learning的一環，在BERT跟GPT出現之前，Auto-Encoder就出現了！
2. Auto-Encoder算是self-supervised learning的其中一種方法！
3. Auto-Encoder如何運作？

   有兩個Network(encoder & decoder)，訓練的目標是希望encoder的輸入跟decoder的輸出越接近越好(跟Cycle GAN的概念其實是一模一樣的)

   訓練過程不需要任何有標註的資料，只要收集到大量的資料即可
4. 怎麼把Train完的Auto-Encoder放在downstream mission裡呢？

   圖片經過Encoder的壓縮之後，不再是一個很高維度的向量，而是一個較低維度的向量(dimension reduction)，再拿此低維度的向量來做後面想做的事情！
5. Auto-Encoder到底好在哪裡？

   因為圖片的變化是有限的，所以在做Encoder的時候，可以用較低的維度去描述原本的那張圖片

   

