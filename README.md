# ロボットシステム学　課題１

---

### 課題内容

第７回、第８回で作成したデバイスドライバーを改造し、オリジナルのものをGitHubに置く。  
また、デバイスドライバーでデバイスを動かしている様子を撮影しYouTubeに公開する。

---

### オリジナルデバイスドライバー　説明

コード：[https://github.com/ChinaMihara/RobotSystemTask1/blob/main/myled/myled.c](https://github.com/ChinaMihara/RobotSystemTask1/blob/main/myled/myled.c)  
  
LED５つを点滅させ信号機(車道用、歩道用)を表現しました。  
echo 0 > /dev/myled0 : 全LED消灯  
echo 1 > /dev/myled0 : LED点滅  

---

### 使用した物

・Raspberry Pi 4 Model B/4GB ×1  
・ブレットボード　×1  
・LED(緑) ×2  
・LED(赤) ×2  
・LED(黄) ×1  
・抵抗　220Ω ×5  
・ジャンパー線 ×10  

---
### 実行手順 
・git clone  https://github.com/ChinaMihara/RobotSystem-Task1.git  
・cd RobotSystem-Task1/  
・cd myled/  
・sudo insmod myled.ko  
・sudo chmod 666 /dev/myled0  
・echo [0 or 1] > /dev/myled0  
  
※「1」を入力した際はLEDが点灯したまま終了するため最後に「0」を入力してください。

---
### 動画
[https://youtu.be/3yTn8k5FCRs](https://youtu.be/3yTn8k5FCRs)
