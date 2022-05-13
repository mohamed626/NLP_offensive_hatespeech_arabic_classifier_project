# NLP_offensive_hatespeech_arabic_classifier_project
detect tweets that have offensive and hatespeech 


## preprocessing
  -deal with nulls
  -deal with categorical data like(NOT_OFF, OFF, NOT_HS,HS6, HS1, HS3, HS5, HS2, NOT_VLG,VL NOT_VIO,VIO) <br>
  -remove useless strings [punc, numbers, tashkeel, extra white spaces]<br>
  -translate franco <br>
  -remove english characters<br>
  -remove redundant ex. hhhhhhh -> h <br>
  -covert emoji to meaningful arabic text ex. 😔 -> وجه حزين



<br>
## task A (offensive orr not)

# GRU model on imbalanced data  
<br>
--model <br>
the GRU model
![image](https://user-images.githubusercontent.com/61325915/168397609-2894123b-a712-4745-81cd-e7edb2f12148.png)

<br>
--data  <br>
we used GRU model on the original dataset wich was imbalanced data with our word embedding using supervised 
![image](https://user-images.githubusercontent.com/61325915/168397418-e84f48a3-8c7c-459d-bc20-ecd84a06765a.png)
<br>
--result  <br>
the model score 0.69 for F1 score wich was the metric for the competition
<br>![image](https://user-images.githubusercontent.com/61325915/168398264-b6b0dd73-9564-446c-9168-f062a3a08a52.png)

<br>
![image](https://user-images.githubusercontent.com/61325915/168398301-b8e349c4-f653-413b-b80f-fce08069865c.png)





## we will focus on task A and task B in this project (offensive,hatespeech)



we used GRU to detect the offensive tweets we apllied the GRU on the data where it imbalanced and after we 
  
