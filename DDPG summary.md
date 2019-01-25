## 공부시 유의할점
#### soft update에 관하여
target network 는 critic 학습 방향이 흔들리지 않도록 하기 위한 수단이다. DQN 에서는 target network를 고정시켜두고 그 방향으로 main network 학습을 진행하며 일정 step 마다 한번씩 main network의 w를 target network로 그대로 복사하는데, DDPG 에서는 매 step soft update 한다. 이 soft update로 인해 target network의 w는 main networkdml w 방향으로 매 step 조금씩 이동한다.

## one picture
![ddpg](https://user-images.githubusercontent.com/9976453/51683122-724fe800-202c-11e9-8e72-97eb538584b2.png)
