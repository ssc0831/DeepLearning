# DeepLearning(DL) 소스코드

### California_Housing(기존 07-03 코드 에러로 수정한 것)

### 09-06 실행시 에러(수정할 필요가 있음)

### 13-03 약간 수정

### 13-07 GPU로 구동시 마지막에 변경할 점(CPU 수정파일 참고)
- confusion_matrix_np = confusion_matrix(y[-1].cpu(), torch.argmax(y_hat.cpu(), dim=-1))로 수정해줘야 함.

### 14-06 GPU로 구동시 마지막에 변경할 점(CPU 수정파일 참고)
- pd.DataFrame(confusion_matrix(y[-1].cpu(), torch.argmax(y_hat.cpu(), dim=-1))

### 15-practical_exercise
- train.py 구현 (conda install pytorch torchvision)
- predict.ipynb(수정)
- predict.ipynb에서 model.pth에서 tmp.pth로 수정
- model.py, tmp.pth 파일을 content에 넣어줘야 적용 됨(Colab 사용시)

### 16,17 Pass

### 18-cnn
- train.py 구현
- predict.ipynb(수정)
- train.py로 만든 model.pth를 content로 이동 시키기
- mnist_classifier 폴더 생성 trainer.py utils.py 이동
- 하위 폴더로 models 폴더 생성 cnn.py fc.py 이동
혹은 import sys 앞쪽에
- from google.colab import drive
- drive.mount('/content/drive')
- %cd /content/drive/MyDrive/Colab Notebooks/BigData DeepLearning/DeepLearning 소스코드/실습/18-cnn
- Colab의 드라이브 마운트 시켜줘야 함.

