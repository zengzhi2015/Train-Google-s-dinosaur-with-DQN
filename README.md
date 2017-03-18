# Train-Google-s-dinosaur-with-DQN

## game play
包含了用于获取人类游戏数据的脚本。

+ count.py
  - 获取**transition**的总数
+ capture.py
  - PIL 截取屏幕（仅windows可用）
  - pyHook 监控按键
  - pickle 将数据序列化
  - 数据存储在 `./game play/human/`
+ gameoverCLF.py
  - 用于判断截屏是不是game over
+ analyze.ipynb
  - 提供简易分析，检查capture是否符合DQN的要求
+ preprocess.ipynb
  - 对截屏进行预处理，转化成可供DQN直接学习的transition
  - 从`./game play/human/`提取文件，处理完毕后，存储在`./game play/transitions/`
