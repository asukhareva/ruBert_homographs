# ruBert_homographs
Fine-tuning ruBert for the task of placing accents in homographs for Yandex competition 2021
## Solution
ruBert is applied in NER mode. Each word will be marked according to the following rule: 
1. if the word is a homograph, then tag B- + word with a homograph;
2. otherwise tag O.
   
Next, the classification problem is solved for each token. There are as many classes as there are different homographs + token O.
## Mitric
Accuracy >= 0.95
