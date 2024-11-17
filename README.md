

# OverView of the Project


1. Opening background information (내 프로젝트의 전반적인 문맥을 위해서 필요!)

2. General description of the current project (프로젝트의 전반적인 설명)

3. Proposed idea for enhancements to the project (제안하고 싶은 프로젝트의 강점)

4. Value and significance of this project (중요성)

5. Current limitations (직면하고 있는 한계)

6. Literature review (전반적인 프로젝트의 배경지식 공유를 위해서)



## 1 .Opening Background Information 

* Table tennis is one of the most popular sports worldwide, where technique and strategy play crucial roles. 
As a result, there is a growing demand for improved methods of match analysis and training.
With advancements in AI technology, the ability to analyze data and react in real time during matches has become a possibility. 
Based on this context, the aim of this project is to develop a system that uses AI to detect and analyze the movement of a table tennis ball.  

## 2. General Description of the Current Project

- The current project aims to develop a system using YOLOv5 (Object Detection Model) to detect table tennis balls in real-time.
This system analyzes footage captured by high-speed cameras to track the position and movement of the ball.
By doing so, it generates data that can be used to assess players' techniques, such as swings, serves, and other skills, providing valuable feedback during training sessions to improve performance.


## 3. Proposed Idea for Enhancements to the Project

- The strength of this project lies in leveraging the high accuracy and speed of YOLOv5, enabling real-time data analysis.
In the future, we plan to enhance the system by integrating additional machine learning algorithms to predict the trajectory of the table tennis ball and analyze match strategies.
Additionally, we will improve the user interface (UI) to make it more accessible for players and coaches, thereby increasing the system’s practicality and ease of use.

## 4. Value and Significance of This Project 

- This project has the potential to become a valuable tool for enhancing the skills of table tennis players. By leveraging AI for objective data analysis, it maximizes the efficiency of training sessions.
Additionally, the data-driven feedback system can analyze individual players’ performances and assist in developing customized training programs. 
This not only contributes to the advancement of table tennis as a sport but also expands the application possibilities of data analysis technologies in other areas.

## 5. Current Limitations 

- The current system has a few limitations. First, the accuracy of ball detection may decrease under varying lighting conditions or complex backgrounds.
Second, tracking becomes challenging when multiple balls are present simultaneously in the frame, leading to potential confusion in object detection. 
Third, there is a need to improve the real-time processing speed of the system, which may require enhancements in hardware performance to ensure efficient handling of high-speed data streams. 
Addressing these limitations will be crucial for the system’s effectiveness in practical training environments.


## 6. Literature Review

- Existing research on table tennis ball recognition primarily focuses on high-speed object detection using computer vision and deep learning models.

- YOLO Series: The YOLO (You Only Look Once) algorithm, introduced by Redmon et al., is a model capable of rapidly detecting objects in a single network pass, demonstrating high performance in real-time object recognition. The latest version, YOLOv5, further enhances speed and accuracy, making it suitable for deployment on edge devices.
Edge Computing: Edge AI platforms like the Nvidia Jetson series allow high-performance AI tasks to be performed with low power consumption, enabling real-time data processing without relying on cloud services.
Sports Data Analysis: AI-powered analysis systems have already been adopted in sports such as soccer, basketball, and tennis, where they contribute to improving player performance and strategy analysis. For sports like table tennis, which require rapid reactions, precise data collection and analysis are crucial.
References:

- Redmon, J., Farhadi, A., "YOLOv3: An Incremental Improvement", 2018.
Bochkovskiy, A., Wang, C.-Y., Liao, H.-Y. M., "YOLOv4: Optimal Speed and Accuracy of Object Detection", 2020.
Nvidia Developer Documentation on Jetson Nano/Xavier.


## Dataset acquisition process

### 1.https://universe.roboflow.com/ Go to the link

![스크린샷(29)](https://github.com/user-attachments/assets/e06a3a05-17bc-4689-a5bc-f41921570d2e)

### 탁구공 데이터 셋을 찾아서 yolov5 데이터셋을 다운받아줍니다.

![스크린샷(30)](https://github.com/user-attachments/assets/bc8e158b-64bc-4a56-8800-ed48ed153046)
![스크린샷(43)](https://github.com/user-attachments/assets/974e4c21-c8e3-41e1-88e5-3d406367d365)

### Google Colaboratory 를 사용하여 코드를 작성해줍니다.

### 1.구글 드라이브 연동

### 코랩에서 구글드라이브 와 연결해줍니다.
![스크린샷(34)](https://github.com/user-attachments/assets/a7f4426b-68b5-49be-a673-c073272c07f2)

### 2.yolov5 설치
### yolov5를 설치해줍니다.
![스크린샷(47)](https://github.com/user-attachments/assets/e914556a-a768-4e79-bd89-1dfab27556cf)

### 3.이미지 파일관리

### 이미지파일을 관리할 폴더를 생성해줍니다.
![스크린샷(36)](https://github.com/user-attachments/assets/0bbb8d2e-55fb-44b8-899f-ed0b27ec426d)

### roboflow 에서 받은 data 파일들을 경로에 알맞게 넣어줄겁니다.
![스크린샷(31)](https://github.com/user-attachments/assets/d7fff744-6e16-49dd-aa1f-8d72a143f434)
### roboflow 에서 받은 data.yml 파일은 수정해줘야됩니다
![스크린샷(48)](https://github.com/user-attachments/assets/a975947b-36d4-4b35-bc3a-32a154655d77)

![스크린샷(46)](https://github.com/user-attachments/assets/1684c4dc-ea7b-41a1-8a93-f866c1369c4e)
### 위의 사진들과 처럼 넣어주면 됩니다


### 검증데이터를 생성합니다.

![스크린샷(37)](https://github.com/user-attachments/assets/4f7c1df9-6864-4c13-877c-a25fbb20adca)

![스크린샷(38)](https://github.com/user-attachments/assets/59eba4c0-a985-47c6-9647-e3c4c0a34cf1)

### 필요라이브러리를 불러옵니다

![스크린샷(39)](https://github.com/user-attachments/assets/7b43e8ce-0892-4ec8-8a8e-1a678d8ab9c9)

![스크린샷(40)](https://github.com/user-attachments/assets/06fcbfbe-5ff1-4211-a824-c8c8571ddfb3)

### 학습시킵니다

![스크린샷(41)](https://github.com/user-attachments/assets/806bdfbf-6bf8-429b-8869-2ac7a289e62e)

### 학습결과

![스크린샷(17)](https://github.com/user-attachments/assets/3f26ff60-6aae-4fe4-8c6c-fd8a33bd2f80)

![스크린샷(18)](https://github.com/user-attachments/assets/2b57f3cd-7c9a-415a-847a-7cc58ff941d3)

![스크린샷(19)](https://github.com/user-attachments/assets/2f58aa1c-e583-4363-95f7-a53c88abe2a8)

![스크린샷(20)](https://github.com/user-attachments/assets/f303af50-2c19-470d-a142-4628be8268e1)

![스크린샷(21)](https://github.com/user-attachments/assets/68f990c1-0f71-44bf-af2a-01e310d1a837)


## 검증 영상입니다.


https://github.com/user-attachments/assets/a27725c2-28e2-47f5-aedc-d35557f111ba


https://github.com/user-attachments/assets/80e42731-abec-4f31-aad6-71078a8ef8a2










