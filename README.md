## Face_recognition 
 - Dlib library example Python - Face recognition
 - OpenCV
 - Python
 - Thonny
 
## Features
 - 기존에 저장된 파일과 비교할 사진을 입력 받아 얼굴의 위치를 탐지
 - 미리 학습된 모델을 통해 탐지된 얼굴에서 68개의 Landmark를 찾음.

   ![Capture](https://raw.githubusercontent.com/colle123/Face_recognition/main/Capture/Code1.jpg)
   
 - 해당 점들의 Landmark들의 위치정보를 기반으로 128개의 비교 표본을 생성(Encording)
 - 비교 표본간 거리(Threshold)가 0.35이하이면 해당 인물로 판별, 0.35보다 크다면 Unknown으로 화면에 표기

 
## Result
   ![Success](https://raw.githubusercontent.com/colle123/Face_recognition/main/Capture/Success.JPG)
   
   카메라로 얼굴을 촬영했지만 아직 인식하지 못하여 화면에는 Unknown이 표시되고 서보모터가 회전하지 않음
   
   <br/>
   
   ![Success1](https://raw.githubusercontent.com/colle123/Face_recognition/main/Capture/Success2.JPG)
   
   얼굴인식에 성공하여 사진 아래에 이름이 'Suhan'으로 바뀐 뒤 서보모터가 회전 된 것을 확인할 수 있음
   
   <br/>
   
   ![Fail](https://raw.githubusercontent.com/colle123/Face_recognition/main/Capture/Fail.JPG)
   
   다른사람이 카메라에 캡쳐되면 Unknown으로 표시되며서보모터가 회전하지 않음
