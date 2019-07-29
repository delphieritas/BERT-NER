# BERT-NER

**\*\*\*\*\*  Jul 27st, 2019  \*\*\*\*\**

## Usage
Pls use 'bash run_ner.sh' in MAC terminal or Linux (Ubuntu/...).
The model is trained on data\train.txt (based on conll2003 dataset).
To test the model performance, feed the model with your test dataset. Refer to data\test.txt for the dataset format.
The Tag Description is following this website: https://www.ling.upenn.edu/courses/Fall_2003/ling001/penn_treebank_pos.html

## Output
A sample output is given, which was tested on NUS SoC tagged dataset, data\test.txt (600+ sentences, most are collected from the latest Bloomberg news dated to Jul 2019). And the model was trained on the data\train.txt (conll2003).         

processed 10368 tokens with 652 phrases; found: 670 phrases; correct: 483.
|Acuracy:  | 97.12% | precision: | 72.09% | recall:  | 74.08% |  FB1:  | 73.07  |
|--------- |------- |------------|--------|----------|--------|--------|--------|                
|          | LOC:   | precision: | 92.71% | recall:  | 95.70% |  FB1:  | 94.18  |192                           
|          | MISC:  | precision: | 63.44% | recall:  | 76.13% |  FB1:  | 69.21  |186                             
|          | ORG:   | precision: | 70.63% | recall:  | 64.96% |  FB1:  | 67.68  |126                         
|          | PER:   | precision: | 59.04% | recall:  | 56.32% |  FB1:  | 57.65  |166                   
              
## Note:
Do not remove the file, label_test.txt (under dir: output\result_dir), which is required when performing the training and testing.
The original BERT repo can be found https://github.com/google-research/bert                      
The BERT-NER repo is based on code provided here https://github.com/kyzhouhzau/BERT-NER
