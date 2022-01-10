## 실습2 : 오픈소스예제 ROS 패키지화

### 개요



### 실행

```
ros2 run turtlesim turtlesim_node

ros2 service call /spawn turtlesim/srv/Spawn "{x: 1.0, y: 1.0, theta: 0.0, name: 'turtle2'}"

ros2 run turtle_dwa control
```
