# 2023_2_opensw_201810991
1. docker pull tensorflow/tensorflow:2.2.0-gpu
이미지 pull

2. docker run -dit --name tensor tensorflow/tensorflow:2.2.0-gpu
도커 run

3. docker exec -it tensor /bin/bash
도커 접속

4. apt-get update
패키지 업데이트

5. apt-get install git
git 설치

6. apt-get install vim
vim 설치

7. apt-get install wget
wget 설치

8. cd /home
홈디렉토리로 이동

9. git clone https://github.com/akTwelve/Mask_RCNN.git aktwelve_mask_rcnn
마스크 CNN 클론

10. cd aktwelve_mask_rcnn/
마스크CNN 디렉토리 이동

11. vi requirements.txt
vi로 requirements.txt수정

12. tensorflow>=2.0.0 열 삭제

13. opencv-python을 opencv-python==4.1.2.30로 수정

14. shift+; 후 wq + Enter로 저장 후 종료

15. pip install -r requirements.txt
의존성 및 패키지설치

16. python setup.py clean --all install
mask R-Cnn설치

17. wget https://github.com/matterport/Mask_RCNN/releases/download/v2.1/mask_rcnn_balloon.h5
가중치 파일 다운로드

18. cd samples/balloon/
ballon sample 디렉토리 이동

19. wget https://github.com/matterport/Mask_RCNN/releases/download/v2.1/balloon_dataset.zip
데이터셋 다운로드

20. unzip balloon_dataset.zip
압축해제

21. python3 balloon.py splash --weight=../../mask_rcnn_balloon.h5 --image=balloon/val/14898532020_ba6199dd22_k.jpg
balloon실행

22. 해당 디렉토리에 나온 splash로 시작하는 파일이 결과값.
