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

![image](https://img2018.cnblogs.com/blog/1538832/201907/1538832-20190714224844251-1534150405.png)

3.建立新的Colab 筆記（Notebook），透過右鍵點擊> More > Colaboratory 步驟建立一個新的筆記<br />

![image](https://img2018.cnblogs.com/blog/1538832/201907/1538832-20190714225153623-189155043.png)

透過點擊檔案名稱來重新命名筆記<br />

![image](https://img2018.cnblogs.com/blog/1538832/201907/1538832-20190714225240840-1044399482.png)

4.打開GPU<br/>
  Edit > Notebook settings或進入Runtime > Change runtime type，然後選擇GPU作為Hardware accelerator（硬體加速器）。

![image](https://img2018.cnblogs.com/blog/1538832/201907/1538832-20190714225413657-1785459503.png)

5.使用Google Colab 運行基本的Python 程式碼<br />
  這個倒是不常用，使用這個功能類似jupyter notebook，而我們要跑的程式碼基本上是已經編輯好的工程項目。利用colab主要是想透過GPU加速更快的訓練。

![image](https://img2018.cnblogs.com/blog/1538832/201907/1538832-20190714225610556-1791273060.png)

6.在建立的資料夾頁面上傳你的整個要跑的檔案(包括資料集)，右鍵選取upload fold 或直接拖曳也行

<br />

Colab 模型訓練
<br />
1.載入磁碟 <br />

from google.colab import drive
drive.mount('/content/drive/')
fs

2.切換到你要跑的目錄下面 <br />

# 指定当前的工作文件夹
import os
# 此处为google drive中的文件路径,drive为之前指定的工作根目录，要加上os.chdir("/content/drive/MyDrive/LapSRN/") 

<br />
3.安裝Pytorch以及torchvision <br />
Colab 一般情況下已經自備了pytorch環境了。若沒有可以進行對應的安裝：

!pip install torch torchvision  # 在Colab中执行操作语句时，感叹号不能漏<br />

4.執行訓練命令 <br />

fs

5.注意事項 <br />
最重要的是路徑問題，一般在data.py或dateset.py檔案裡面有關於路徑的，還有save model時候。可以將路徑相關的都改成parse的語句，在執行指令時傳入防止出錯。相關的路徑可以直接複製
































