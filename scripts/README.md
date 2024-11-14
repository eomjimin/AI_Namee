# 모델 학습 및 데이터 정제 코드

## 데이터 정제 코드
- make_faiss.py: faiss DB를 생성하는 코드
- db_dataset.py: faiss DB안에 넣을 회의록을 정제하는 코드
- finetuning_dataset.py: NER을 위해 llm 모델을 finetuning 하기 위해 사용된 데이터셋

## 모델 학습 코드
- Meta사의 https://github.com/meta-llama/llama-recipes.git 코드를 task에 맞게 단순화 및 refactoring 하여 finetuning 진행
- input과 output의 쌍으로 이루어진 딕셔너리들을 학습 데이터로 사용
- learning-rate: 2e-4, 30 epoch으로 학습 진행