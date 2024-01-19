# EMS.Yolo
mobiler roboter




1.Erstellung eines virtual environment

  $  pip install virtualenv
  
  $  virtualenv --python=/usr/bin/python3 myenv_yolo
  
  $  source myenv_yolo/bin/activate
  

  zur Deaktivierung  von myenv_yolo
  
  $  deactivate

  

2.Installierung benötigter Bibliotheken

  $ pip install lida==0.0.1
  
  $ pip install ultralytics==8.0.196
  
  $ pip install supervision
  
  $ pip install roboflow
  
  $ pip install inference
  
  $ pip install testresources
  
  $ pip install fastapi kaleido python-multipart uvicorn

  

3.Package erstellen 

  cd ~/catkin_ws/src/myenv_yolo
  
  $ catkin_create_pkg your_package_name roscpp rospy std_msgs

  

4.Zur Authentifizierung des API_KEYs in myenv_yolo

  export ROBOFLOW_API_KEY="api-key"


5.yolo.py file in environment implementieren als code, sodass dieser
mit den folgenden befehl angesprochen werden kann.

  $ rosrun ems yolov8.py
