# NLP_offensive_hatespeech_arabic_classifier_project
detect tweets that have offensive and hatespeech 


<br>
## Link dataset: https://alt.qcri.org/resources/OSACT2022/OSACT2022-sharedTask-train.txt
<br>

## preprocessing
  -deal with nulls
  -deal with categorical data like(NOT_OFF, OFF, NOT_HS,HS6, HS1, HS3, HS5, HS2, NOT_VLG,VL NOT_VIO,VIO) <br>
  -remove useless strings [punc, numbers, tashkeel, extra white spaces]<br>
  -translate franco <br>
  -remove english characters<br>
  -remove redundant ex. hhhhhhh -> h <br>
  -covert emoji to meaningful arabic text ex. 😔 -> وجه حزين



<br>
## task A (offensive orr not) poor accuracy cause of small very noisy data

# GRU model on imbalanced data   F1 score =0.69
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
the model score 0.69 for F1 score wich was the metric for the competition <br>
classification report
<br>![image](https://user-images.githubusercontent.com/61325915/168398264-b6b0dd73-9564-446c-9168-f062a3a08a52.png)

<br>
confusion matrix <br>
![Capture](https://user-images.githubusercontent.com/61325915/168398656-979a35d3-d94a-4b05-b9e4-bec23a9d5b94.PNG)




# GRU model on balanced data (undersampled)  F1 score =0.69
<br>
--model <br>
the GRU model
![image](https://user-images.githubusercontent.com/61325915/168397609-2894123b-a712-4745-81cd-e7edb2f12148.png)

<br>
--data  <br>
we used GRU model on the original dataset wich was imbalanced data with our word embedding using supervised 
![image](https://user-images.githubusercontent.com/61325915/168398978-f0534aa3-4985-4aee-aecc-a11de6524991.png)<br>

--result  <br>
the model score 0.69 for F1 score wich was the metric for the competition <br>
classification report
<br>![image](https://user-images.githubusercontent.com/61325915/168399088-04ba68fd-0646-44be-8378-2c43712aed0b.png)

<br>
confusion matrix <br>
![image](https://user-images.githubusercontent.com/61325915/168399111-c97b4c26-dde2-4b6b-989b-f27af743c2ea.png)
<br>






# BERT model imbalanced data  F1 score =0.68
<br>
--model <br>
the BERT model
![image](https://user-images.githubusercontent.com/61325915/168399585-9d76f37a-bcc1-4812-ab3a-bf1e856e539e.png)

<br>
--data  <br>
we used GRU model on the original dataset wich was imbalanced data with our word embedding using supervised 
![image](https://user-images.githubusercontent.com/61325915/168398978-f0534aa3-4985-4aee-aecc-a11de6524991.png)<br>

--result  <br>
the model score 0.68 for F1 score wich was the metric for the competition <br>
classification report
<br>![image](https://user-images.githubusercontent.com/61325915/168399500-a715651f-8733-49f9-b7c3-5f62e522b824.png)

<br>
confusion matrix <br>
![image](https://user-images.githubusercontent.com/61325915/168399523-697051b1-dd67-43ce-849e-075cf30ac663.png)
<br>





# BERT model balanced data (undersampled)  F1 score =0.64
<br>
--model <br>
the BERT model
![image](https://user-images.githubusercontent.com/61325915/168399585-9d76f37a-bcc1-4812-ab3a-bf1e856e539e.png)

<br>
--data  <br>
we used GRU model on the original dataset wich was imbalanced data with our word embedding using supervised 
![image](https://user-images.githubusercontent.com/61325915/168398978-f0534aa3-4985-4aee-aecc-a11de6524991.png)<br>

--result  <br>
the model score 0.64 for F1 score wich was the metric for the competition <br>
classification report
<br>![image](https://user-images.githubusercontent.com/61325915/168399659-b4b06eb4-88d4-4b9e-b8dc-25f408957e7c.png)


<br>
confusion matrix <br>
![image](https://user-images.githubusercontent.com/61325915/168399680-d73b3567-04f3-49d4-a435-f7c628aa481f.png)
<br>







# BERT model balanced data (oversampled)  F1 score =0.36 
<br>
--model <br>
the BERT model
![image](https://user-images.githubusercontent.com/61325915/168399585-9d76f37a-bcc1-4812-ab3a-bf1e856e539e.png)

<br>
--data  <br>
we used GRU model on the original dataset wich was imbalanced data with our word embedding using supervised 
![image](https://user-images.githubusercontent.com/61325915/168398978-f0534aa3-4985-4aee-aecc-a11de6524991.png)<br>

--result  <br>
the model score 0.36 for F1 score wich was the metric for the competition <br>
classification report
<br>![image](https://user-images.githubusercontent.com/61325915/168399848-2682161f-0ce4-4cc8-931e-48fc14b004ab.png)


<br>
confusion matrix <br>
![image](https://user-images.githubusercontent.com/61325915/168399871-e27e7829-fc3e-4aff-9428-520a1ff62f09.png)
<br>




## task B (hatespeech or not) 

# BERT model on imbalanced data  F1  score = .91 on test data 
<br>
--model <br>
the BERT model
![image](https://user-images.githubusercontent.com/61325915/168399585-9d76f37a-bcc1-4812-ab3a-bf1e856e539e.png)

<br>
--data  <br>
we used BERT model on the original dataset used BERT embedding
![image](https://user-images.githubusercontent.com/61325915/168397418-e84f48a3-8c7c-459d-bc20-ecd84a06765a.png)
<br>
<br>
--result  <br>
the model score 0.91 for F1 score wich was the metric for the competition <br>
![image](https://user-images.githubusercontent.com/61325915/168401982-20d3acfe-7dd5-494d-ab15-381d9d3b0ae5.png)



