## 실습1 : Turtlesim을 활용한 ROS 기초 프로그래밍

### 개요

Turtlesim에서 아래 조건을 만족하면서 입력 명령을 받아 거북이를 등속 원운동하게하는 ROS2 패키지를 설계하시오. 

1. 원운동의 회전반경(radius), linear velocity(velocity), 회전방향(direction) 값을 포함하는 ROS 메세지 타입을 정의하고 이 토픽 메세지를 받아 Turtlesim에 속도명령(cmd_vel)을 주는 프로그램을 설계한다. 
2. ros2 launch로 turtlesim과 설계한 프로그램을 동시에 실행할 수 있는 launch 파일을 제작한다. 
3. turtlesim 실행 후, ros2 topic pub으로 새롭게 정의한 메시지 타입을 publish하여 등속 원운동을 명령한다. 
4. C++ / Python등의 언어는 자유롭게 선택하여 진행한다.


### 실행

```
ros2 launch turtle_circle turtle_circle.launch.py
ros2 topic pub /rad_vel_dir turtle_rcle_interfaces/msg/RVD "{radius: 2.0, velocity: 2.0, direction: True}"
```
