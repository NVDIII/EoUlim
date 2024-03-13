# 👋 어울림
##### 실시간 농인과 비장애인 간의 소통 지원 어플
###### 인원: 5명
###### 기간: 2024-02-26 ~ 2024-03-07
-----------------
## 💡 프로젝트 기획
수많은 수어 관련 프로젝트들을 봤지만, 단순하게 단어를 번역해주는 프로젝트들만 다수 존재할 뿐, 실시간으로 소통이 가능하도록 하는 프로젝트는 보지 못함.
수어는 음성으로, 음성은 텍스트로 번역함으로서 하나의 단말기로 농인과 비장애인이 소통할 수 있도록 하고자 함.


<img width="100%" alt="image" src="https://github.com/NVDIII/EoUlim/assets/124571378/17b3748a-604f-4dcd-b88e-6cae5177511a">

<hr>

# **두 가지 데이터로 학습**
영상 데이터와 키포인트 데이터를 각각 다른 방식으로 학습시킴.
YOLO - 영상
ResNet - 키포인트
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/b9041c53-3ddd-45b8-9e93-413379d7bb00">


## 👨‍💻 Process & Role
#### Overall Process
###### - 기획, 서버구현, 프론트구현, 모델학습, 서버배포, PPT제작, 발표, 데이터수집
#### 😺 My Role
###### - 기획, 서버구현, 프론트구현, 서버배포, PPT제작, 데이더수집

## 🌏 Dataset & Model
#### Dataset
- 문제별로 [질문과 답변 데이터](https://github.com/moon-123/Matchuri-NLP-project/files/14344362/QADataset.xlsx)를 직접 작성함
- 모델 학습에 사용한 문제는 총 6개로 2289개의 질문-답 데이터셋 사용

#### Model
- 문장 학습 모델 [skt/kogpt2-base-v2](https://github.com/SKT-AI/KoGPT2)
- 유사도 측정 모델 [ddobokki/klue-roberta-base-nli-sts](https://huggingface.co/ddobokki/klue-roberta-base-nli-sts)
-----------------
## 🚀 Result

### **발표ppt**
[추리추리 마추리 ppt](https://github.com/dev-aram/Mathuri/blob/master/%EB%A7%88%EC%B6%94%EB%A6%AC_%EB%B0%9C%ED%91%9C.pdf)


### **프론트**
- 제작 화면1
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/102acf10-a28f-4910-9cf4-fcbbe411205e">

- 제작 화면2
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/dc70ce0e-efc0-4c11-ba5a-46af259e8fb7">

### **서버**
확장성을 위해 node, python 두가지 서버를 같이 사용 채팅부분을 제외한 나머지 부분은 전무 node.js로 서버를 작업하였고 모델과 소통해야하는 채팅 부분은 python 서버로 작업하였습니다.

<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/1abe245c-1cab-4294-9e44-64e31c57926f">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/ca2ee070-ea4b-46e9-85be-62f0dad75699">

### **모델**
유저가 질문을 입력하면 RoBerta로 유사성을 검사하고 문제와 유저가 입력한 질문이 유사하다고 판단되면 GPT2 모델에 넣어 학습한 질문과 대조하여 학습된 답변을 그래도 출력하거나 GPT2가 생성한 답변을 출력되게 모델을 학습시켰습니다.

<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/7be28c64-0c2a-4e17-ab4d-9c0295ba1180">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/dff17a9b-6752-4187-a0f4-8e799135f226">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/28ab16b7-c197-4998-8993-d5dfd0ad3c33">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/49ffe5e3-0676-4e6a-97b9-8b504c6e3f2a">

- **전처리 과정**
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/f08979cc-647c-4085-b13e-6e097dfe9e71">

- **GPT2**
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/4ac6fced-5981-4921-ba5c-487182f1af63">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/8ad2ec6f-2fb0-49e4-adaa-20f6299589de">
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/4bbd766f-4db5-4ebd-9524-9dcf0ea4250d">

- **최종모델**
<img width="100%" alt="image" src="https://github.com/dev-aram/Mathuri/assets/135501045/4dc61506-bd8a-45b1-bcfd-2a6b23431b69">



-----------------
### ⚙️ Skills & Tools

<p>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/JavaScript-gray?style=flat&logo=JavaScript&logoColor=F7DF1E"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=4479A1"/>&nbsp;&nbsp;
</p>

<p>
  <img src="https://img.shields.io/badge/Colab-F37626?style=flat&logo=googlecolab&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/VScode-007ACC?style=flat&logo=visualstudiocode&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/Discord-5865F2?style=flat&logo=Discord&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/AWSEC2-FF9900?style=flat&logo=amazonec2&logoColor=white"/>&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/AWSS3-569A31?style=flat&logo=amazons3&logoColor=white"/>&nbsp;&nbsp;

  
</p>
