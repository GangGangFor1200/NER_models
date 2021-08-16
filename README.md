# NER_models

21.08.16 BERT-CRF, BERT-BiLSTM-CRF 모델 추가, 작동확인

## BERT-CRF

### sample data 오류 수정
https://github.com/devjwsong/bert-crf-entity-recognition-pytorch/issues/1

### bert_config.dim 오류 수정
```
# original
self.config['hidden_size'] = bert_config.dim

# fixed
self.config['hidden_size'] = bert_config.hidden_size
```
## BERT-BiLSTM-CRF
중국어-> 한국어 fine-tuning 필요


