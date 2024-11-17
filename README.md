# Nvidia-AI-Specialist-Certification
OverView of the Project

프로젝트 개요

1. Opening background information (내 프로젝트의 전반적인 문맥을 위해서 필요!)

2. General description of the current project (프로젝트의 전반적인 설명)

3. Proposed idea for enhancements to the project (제안하고 싶은 프로젝트의 강점)

4. Value and significance of this project (중요성)

5. Current limitations (직면하고 있는 한계)

6. Literature review (전반적인 프로젝트의 배경지식 공유를 위해서)

프로젝트 개요

1. Opening Background Information  (내 프로젝트의 배경 정보)

Table tennis is one of the most popular sports worldwide, where technique and strategy play crucial roles. 
As a result, there is a growing demand for improved methods of match analysis and training.
With advancements in AI technology, the ability to analyze data and react in real time during matches has become a possibility. 
Based on this context, the aim of this project is to develop a system that uses AI to detect and analyze the movement of a table tennis ball.  

탁구는 전 세계적으로 인기 있는 스포츠 중 하나로, 기술과 전략이 중요한 요소로 작용합니다. 이에 따라 탁구 경기의 분석과 훈련 방법에 대한 수요가 증가하고 있습니다. 특히, AI 기술의 발전으로 인해 경기 중의 데이터를 실시간으로 분석하고 반응할 수 있는 가능성이 열렸습니다. 본 프로젝트는 이러한 배경을 바탕으로, AI를 활용하여 탁구공을 인식하고 분석하는 시스템을 개발하고자 합니다.

2. General Description of the Current Project(프로젝트의 전반적인 설명)

The current project aims to develop a system using YOLOv5 (Object Detection Model) to detect table tennis balls in real-time.
This system analyzes footage captured by high-speed cameras to track the position and movement of the ball.
By doing so, it generates data that can be used to assess players' techniques, such as swings, serves, and other skills, providing valuable feedback during training sessions to improve performance.




3. Proposed Idea for Enhancements to the Project(제안하고 싶은 프로젝트의 강점)
4. 
The strength of this project lies in leveraging the high accuracy and speed of YOLOv5, enabling real-time data analysis.
In the future, we plan to enhance the system by integrating additional machine learning algorithms to predict the trajectory of the table tennis ball and analyze match strategies.
Additionally, we will improve the user interface (UI) to make it more accessible for players and coaches, thereby increasing the system’s practicality and ease of use.

5. Value and Significance of This Project 

This project has the potential to become a valuable tool for enhancing the skills of table tennis players. By leveraging AI for objective data analysis, it maximizes the efficiency of training sessions.
Additionally, the data-driven feedback system can analyze individual players’ performances and assist in developing customized training programs. 
This not only contributes to the advancement of table tennis as a sport but also expands the application possibilities of data analysis technologies in other areas.

5. Current Limitations 

The current system has a few limitations. First, the accuracy of ball detection may decrease under varying lighting conditions or complex backgrounds.
Second, tracking becomes challenging when multiple balls are present simultaneously in the frame, leading to potential confusion in object detection. 
Third, there is a need to improve the real-time processing speed of the system, which may require enhancements in hardware performance to ensure efficient handling of high-speed data streams. 
Addressing these limitations will be crucial for the system’s effectiveness in practical training environments.


6. Literature Review

Existing research on table tennis ball recognition primarily focuses on high-speed object detection using computer vision and deep learning models.

YOLO Series: The YOLO (You Only Look Once) algorithm, introduced by Redmon et al., is a model capable of rapidly detecting objects in a single network pass, demonstrating high performance in real-time object recognition. The latest version, YOLOv5, further enhances speed and accuracy, making it suitable for deployment on edge devices.
Edge Computing: Edge AI platforms like the Nvidia Jetson series allow high-performance AI tasks to be performed with low power consumption, enabling real-time data processing without relying on cloud services.
Sports Data Analysis: AI-powered analysis systems have already been adopted in sports such as soccer, basketball, and tennis, where they contribute to improving player performance and strategy analysis. For sports like table tennis, which require rapid reactions, precise data collection and analysis are crucial.
References:

Redmon, J., Farhadi, A., "YOLOv3: An Incremental Improvement", 2018.
Bochkovskiy, A., Wang, C.-Y., Liao, H.-Y. M., "YOLOv4: Optimal Speed and Accuracy of Object Detection", 2020.
Nvidia Developer Documentation on Jetson Nano/Xavier.


Dataset acquisition process

1.https://universe.roboflow.com/ Go to the link


탁구공 데이터 셋을 찾아서 yolov5 데이터셋을 다운받아줍니다.



다운받은 탁구공 데이터셋을 yolov5안에 넣어줍니다


data.yml 파일을 경로에 맞게 수정해줍니다.
사진

그후에 검증데이터를 생성해줍니다.
사진

학습시작합니다.
사진

학습 결과물 확인
사진

학습결과물 검증 영상

사진 영상
