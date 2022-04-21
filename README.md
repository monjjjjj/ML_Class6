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


   

