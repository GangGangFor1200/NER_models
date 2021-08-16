# NER_models

21.08.16 BERT-CRF, BERT-BiLSTM-CRF 모델 추가, 작동확인

## BERT-CRF

### sample data 오류
https://github.com/devjwsong/bert-crf-entity-recognition-pytorch/issues/1

사용가능
- sports.txt
- restaurant-search.txt
- food-ordering.txt

restaurant-search.txt 랑 관련있으니 이거로 해보기

### bert_config.dim 오류 수정
```
# original
self.config['hidden_size'] = bert_config.dim

# fixed
self.config['hidden_size'] = bert_config.hidden_size
```
## BERT-BiLSTM-CRF
중국어-> 한국어 fine-tuning 필요


