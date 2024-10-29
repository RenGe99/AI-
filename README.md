## AI-期中報告
組員:11225035謝詠任、11225017黃誠睿
<br />
<br />
 #Colab 實用教程
<br />
目錄

1.Colab是什麼？

2.Colab的基本配置

3.Colab 模型訓練

4.進階使用

<br />
Colab是什麼？
 
 <br />

1.Google Colab 是一個免費的雲端服務並支援免費的GPU，可以：
1-1 提升你的Python語言的程式設計技能。<br />
1-2 使用Keras、TensorFlow、PyTorch和OpenCV等流行庫開發深度學習應用程式。<br />
1-3 Colab 與其它免費的雲端服務最重要的區別在於：Colab提供完全免費的GPU，為學生黨進行AI學習提供便利。<br />

<br />

2.Colab 是Google的且伺服器在國外<br />
2-1 如果不能使用Google，建議使用Kaggle（國內也能使用）👉免費的深度學習GPU環境Colab和Kaggle搭配使用<br />
2-2如果可以上Google，那就繼續往下看學習Colab用法！

<br />
Colab的基本配置<br />
1.登入Google Drive<br />
2.在Google Drive 上建立資料夾，我建立的是名字為app 的資料夾<br />

![image](https://github.com/RenGe99/AI-/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%20(56).png?raw=true)

3.建立新的Colab 筆記（Notebook），透過右鍵點擊> More > Colaboratory 步驟建立一個新的筆記<br />

![image](https://github.com/RenGe99/AI-/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%20(57).png?raw=true)

透過點擊檔案名稱來重新命名筆記<br />

![image](https://github.com/RenGe99/AI-/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%20(59).png?raw=true)

4.打開GPU<br/>
  Edit > Notebook settings或進入Runtime > Change runtime type，然後選擇GPU作為Hardware accelerator（硬體加速器）。

![image](https://github.com/RenGe99/AI-/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%20(61).png?raw=true)

5.使用Google Colab 運行基本的Python 程式碼<br />
  這個倒是不常用，使用這個功能類似jupyter notebook，而我們要跑的程式碼基本上是已經編輯好的工程項目。利用colab主要是想透過GPU加速更快的訓練。

![image](https://github.com/RenGe99/AI-/blob/main/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%20(62).png?raw=true)

6.在建立的資料夾頁面上傳你的整個要跑的檔案(包括資料集)，右鍵選取upload fold 或直接拖曳也行

<br />
Colab 模型训练<br />
1.加载盘<br />

![image](https://github.com/RenGe99/AI-/blob/main/1.jpg?raw=true)<br />

![image](https://github.com/RenGe99/AI-/blob/main/2.png?raw=true)<br />

2.切换到你要跑的目录下面<br />
![image](https://github.com/RenGe99/AI-/blob/main/3.jpg?raw=true)

3.安装Pytorch以及torchvision<br />
![image](https://github.com/RenGe99/AI-/blob/main/4.png?raw=true)

Colab 一般情况下已经自带了pytorch环境了。若没有可以进行相应的安装<br />
4.执行训练命令<br />
![image](https://github.com/RenGe99/AI-/blob/main/5.png?raw=true)

5.注意事项<br />
最重要的是路径问题，一般在data.py或者dateset.py文件里面有关于路径的，还有save model时候。可以将路径相关的都改成parse的语句，在执行命令时传入防止出错。相关的路径可以直接复制

































