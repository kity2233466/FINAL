# AI換臉技術教學：Deepfake影片製作全攻略
## Table of Contents

重點摘要

+ [AI換臉技術概覽](#AI換臉技術概覽)

+ [ROOP Deepfake工具詳解](#roop-deepfake工具詳解)

+ [在Colab上使用ROOP完整教學](#在cloab上使用roop完整教學)

+ [ROOP價格](#roop價格)

+ [ROOP的優缺點分析](#roop的優缺點分析)

+ [ROOP的核心功能](#roop的核心功能)

+ [ROOP的應用場景](#roop的應用場景)

+ [實際換臉成果](#實際換臉成果)

+ [總結](#總結)

隨著人工智慧技術的飛速發展，**AI換臉技術**也日益成熟，Deepfake影片的製作變得越來越普及。無論是出於娛樂目的，還是為了內容創作，掌握AI換臉技術都能為你帶來更多可能性。本文將帶你深入了解Deepfake技術的原理，並提供詳細的Google Colab教學，讓你輕鬆製作出令人驚艷的AI影片。

# **重點摘要**  

+ AI換臉技術的快速發展與應用。

+ Deepfake技術背後的原理。

+ Google Colab在AI換臉影片製作中的作用。

+ 如何使用ROOP在Google Colab上進行Deepfake。

+ AI換臉技術的潛在風險與倫理考量。

# **AI換臉技術概覽**
## **什麼是AI換臉技術？**

AI換臉技術，又稱**Deepfake技術**，是一種利用人工智慧演算法，將影片或圖片中的人臉替換成另一張臉的技術。它利用深度學習模型，分析原始影片或圖片的人臉特徵，然後將目標臉孔無縫整合到原始素材中，產生以假亂真的效果。

AI換臉技術的應用範圍非常廣泛，從娛樂產業到教育領域，都能看到它的身影。然而，由於其可能被用於製造不實資訊或惡意內容，因此也引發了許多關於倫理和法律方面的討論。

儘管存在爭議，AI換臉技術的發展速度卻不容小覷。隨著演算法的不斷改進和硬體效能的提升，Deepfake影片的製作門檻也越來越低，使得更多人能夠接觸到這項技術。

# **AI換臉技術的運作原理**  

AI換臉技術的核心在於**深度學習**，尤其是**生成對抗網路（GANs）**。GANs由兩個神經網路組成：一個是生成器（Generator），負責生成假的人臉圖片；另一個是對抗器（Discriminator），負責判斷生成的圖片是真是假。

**運作流程大致如下：**

1. **資料收集：** 收集大量原始影片或圖片，以及目標臉孔的素材。

2. **人臉辨識與特徵提取：** 使用人臉辨識演算法，偵測原始影片或圖片中的人臉，並提取其特徵，例如臉部輪廓、眼睛、鼻子、嘴巴等。

3. **模型訓練：** 將收集到的資料輸入GANs模型，訓練生成器生成逼真的人臉圖片。同時，訓練對抗器辨識真假圖片，並將結果反饋給生成器，使其不斷改進生成品質。

4. **臉部替換：** 將訓練好的生成器應用於原始影片或圖片，將原始人臉替換成目標臉孔。這個過程需要仔細調整臉部角度、光線、色彩等，以確保替換後的畫面自然無痕。

5. **後製處理：** 進行一些後製處理，例如平滑邊緣、調整色彩平衡等，以進一步提升影片的真實感。

透過不斷的迭代訓練，GANs模型能夠生成極其逼真的人臉圖片，使得AI換臉技術的成果越來越難以辨別。

# **AI換臉技術的應用**

**AI換臉技術**  的應用非常廣泛，以下列舉幾個常見的例子：

+ **娛樂產業：** Deepfake技術可用於製作電影特效、創建虛擬角色、修改明星的臉部表情等，提升影片的視覺效果和趣味性。線上電影串流服務

+ **教育領域：** Deepfake技術可用於製作歷史人物的影片、模擬不同情境下的對話，提升教學的互動性和吸引力。

+ **內容創作：** Deepfake技術可用於製作個人化的影片、創建獨特的頭像，豐富內容的呈現方式。

+ **社交媒體：** Deepfake技術可用於製作有趣的短片、惡搞朋友，增添社交互動的樂趣。

需要注意的是，AI換臉技術的應用必須遵守法律法規和倫理規範，不得用於製造不實資訊、侵犯他人權益等。

# **ROOP Deepfake工具詳解**

## **ROOP是什麼？**

**ROOP（Real-time Object-Oriented Programming）**
是一個**開源的Deepfake工具**，它可以讓你輕鬆地在影片或圖片中替換人臉。ROOP的特色在於其簡潔易用的介面和快速的處理速度，即使沒有程式設計經驗，也能夠輕鬆上手。ROOP利用預先訓練好的深度學習模型，簡化了AI換臉的流程，讓使用者只需上傳原始素材和目標臉孔，就能快速生成Deepfake影片。

ROOP支援多種作業系統，包括Windows、macOS和Linux。它也提供不同的版本，例如CPU版本和GPU版本，使用者可以根據自己的硬體配置選擇合適的版本。

**ROOP的優勢：**

+ **易於使用：** 簡潔的介面和直觀的操作流程，讓使用者輕鬆上手。

+ **快速處理：** 利用預先訓練好的模型，加速AI換臉的過程。

+ **支援多種平台：** 適用於Windows、macOS和Linux等作業系統。

+ **開源免費：** 免費使用，並可以自由修改和分享。


**ROOP的局限性：**

+ **對硬體要求較高：** 尤其是在處理高畫質影片時，需要較強的GPU效能。

+ **生成品質受限：** 由於使用預先訓練好的模型，生成品質可能不如自行訓練模型。

+ **可能存在倫理問題：** 使用ROOP製作Deepfake影片時，需要注意倫理和法律方面的問題。

# **在Colab上使用ROOP完整教學**

Google Colab是一個**免費的雲端平台**，提供Jupyter Notebook的服務，讓使用者可以在雲端執行Python程式碼。Colab還提供免費的GPU資源，非常適合用於進行深度學習相關的任務。ROOP可以在Google Colab上運行，讓你無需在本地安裝任何軟體，就能製作Deepfake影片。

**以下是在Google Colab上使用ROOP的步驟：**

**注意事項：**

+ 在執行程式碼之前，請確保已經連接GPU。 

+ 修改程式碼中的路徑時，請使用正確的檔案名稱和路徑。

+ AI換臉需要一定的時間，請耐心等待。

1. **開啟Google Colab：** 在瀏覽器中輸入

`colab.research.google.com`

，開啟Google Colab。

2. **創建新的Notebook：** 點擊「新增筆記本」，創建一個新的Jupyter Notebook。

3. **連接GPU：** 點擊「代碼執行程式」、「變更執行階段類型」，在「硬體加速器」下拉選單中選擇「GPU」。

4. **安裝ROOP：** 在Notebook中輸入以下程式碼，並執行：

<img width="509" height="111" alt="image" src="https://github.com/user-attachments/assets/973da2c1-34eb-452d-be25-c22ce2f16bdb" />

5. 下載補丁，輸入以下代碼並執行

`!wget -O fix_roop.py https://raw.githubusercontent.com/kity2233466/roop-colab-fix/main/fix_roop.py`

6. **修正版本:**因為roop在2023年開始停止維護更新，所以與現在的google cloab有版本不符問題，所以我們要修正roop的版本，請輸入以下代碼，並執行

`!pip install -q "numpy<2.0" onnxruntime-gpu==1.17.1 insightface==0.7.3 opencv-python-headless==4.9.0.80 customtkinter tkinterdnd2 opennsfw2`

`!mkdir -p models`

`!wget -q --show-progress -O models/inswapper_128.onnx "https://huggingface.co/ezioruan/inswapper_128.onnx/resolve/main/inswapper_128.onnx"`#這行指令不必換行

`print("\n✅ 第一步完成：環境與你的專屬補丁已就緒。")`

代碼如圖
<img width="1411" height="48" alt="image" src="https://github.com/user-attachments/assets/b55e6a40-323f-406b-9042-63d5d808743c" />
<img width="1366" height="107" alt="image" src="https://github.com/user-attachments/assets/f6c25df8-5820-426e-96f1-b5faa3431d1f" />


+ 會跑出這個畫面

<img width="1911" height="928" alt="image" src="https://github.com/user-attachments/assets/9180e497-c533-45bd-a850-01565ee548e1" />

+ 這時候請重新執行工作階段

![1766547430598_0](https://github.com/user-attachments/assets/4e6c641c-2044-4695-a9ba-88d2d6099d9e)

![1766547471525](https://github.com/user-attachments/assets/27375994-e301-4fa0-b4e1-d79a11b08a7c)

7. **補回缺失及執行修復腳本:**

<img width="939" height="445" alt="image" src="https://github.com/user-attachments/assets/30e61f1f-d856-4805-99f7-c8e1b698ca63" />


8. **上傳影片和圖片：** 將原始影片和目標臉孔的圖片上傳到Colab，並且修改圖片檔名為`face.jpg`;影片檔名為`video.mp4`。

+ 先點選檔案，在畫面左方

![1766501665470](https://github.com/user-attachments/assets/68ba4d2d-6c5e-4e4d-a38e-827e45aa28df)

+ 然後在空白處點擊右鍵，按上傳。會出現第二張圖的畫面，按「確定」

<img width="1919" height="994" alt="image" src="https://github.com/user-attachments/assets/326101b1-220f-4e63-ad73-65716268e597" />

<img width="1846" height="1010" alt="image" src="https://github.com/user-attachments/assets/c0512096-1ef0-4871-8da7-82bf035200d2" />

+ 將檔案更改名稱，修改圖片檔名為`face.jpg`;影片檔名為`video.mp4`。

<img width="1906" height="1052" alt="image" src="https://github.com/user-attachments/assets/e9005346-f313-4672-a983-a73905ca4494" />


9. **在執行前確認檔名是否一致**

<img width="296" height="52" alt="image" src="https://github.com/user-attachments/assets/7aacfdfb-3af8-4f69-8928-3a049749cbd2" />
<img width="226" height="39" alt="image" src="https://github.com/user-attachments/assets/efbc9025-8e1f-4d2e-ba05-e2329c1976cf" />

10. **執行換臉程式碼：** 在Notebook中輸入以下程式碼：

`%cd /content/roop`

`!python run.py \
    --source /content/face.jpg \
    --target /content/video.mp4 \
    --output /content/result.mp4 \
    --execution-provider cuda \
    --frame-processor face_swapper`

指令會是這樣

<img width="750" height="295" alt="image" src="https://github.com/user-attachments/assets/d164a112-d761-4565-b585-9b55a0281b73" />

    
11. **·下載生成影片：** 執行程式碼後，ROOP會自動進行AI換臉。完成後，可以點擊左側的「檔案」圖示，找到「result.mp4」這個檔案並下載到本地。

![1766502631719](https://github.com/user-attachments/assets/895aa2e3-5c1b-4b8e-acd8-14ec44ad7d73)

+ 跟改檔名一樣，同樣按右鍵即可下載檔案  

透過以上步驟，你就可以在Google Colab上使用ROOP，輕鬆製作Deepfake影片。 請務必注意倫理問題。

在Google Colab 介面上需要點選右上方「**連接**」，讓系統連結GPU，以便加速運算。

接著按照教學指示，依序點選程式碼左方的「**播放鍵**」符號，讓程式碼開始執行。

在檔案管理員中，會看到上傳的影片和人像，這時，需要將檔案路徑複製到程式碼中，替換原本的路徑。

確認路徑無誤後，再次點擊「播放鍵」符號，執行換臉程式碼。AI換臉所需的時間，會因為影片長度而有所不同，請耐心等候。

影片處理完成後，可以在檔案管理員中找到換臉後的影片，點擊「**下載**」，儲存到本地電腦中。


## **恭喜你，成功製作了Deepfake影片！**

# **ROOP價格**

## **免費開源**

ROOP 是一個**完全免費**且開源的工具，任何人都可以免費下載、使用及修改。由於是開源專案，社群會不斷進行維護及更新，使用者可以從GitHub 頁面獲取最新的版本。

# **ROOP的優缺點分析**
<kbd>👍 **Pros**

+ 使用者友善的介面，操作簡單直觀

+ 高效率的換臉速度

+ 支援多種影片和圖片格式

+ 完全免費使用，無需支付任何費用

開源專案，可自由修改和客製化<kbd>

<kbd>👎 **Cons**

+ 換臉效果可能不夠完美，有時會出現瑕疵

+ 對硬體配備有一定要求，需要具備獨立顯示卡才能獲得較佳效能

+ 部分進階功能需要具備一定的程式設計基礎才能使用

+ 可能存在倫理爭議，需要謹慎使用<kbd>

# **ROOP的核心功能**
# **主要功能**
ROOP的主要功能包括：

+ **臉部替換:** 
快速準確地將影片或圖片中的人臉替換為指定人臉。

+ **多種模式支援：**
支援單張圖片換臉和影片換臉。

+ **高效率處理：**
利用GPU加速，大幅提升換臉速度。

+ **簡單易用：**
提供使用者友善的介面，操作簡單直觀。

+ **開源免費：**
完全免費使用，並允許使用者自由修改和分發。

# **ROOP的應用場景**
### 實際應用

### ROOP的應用場景十分廣泛，包括：

+ 娛樂影片製作：製作惡搞影片、特效影片等，增加娛樂性。

+ 個人化內容創作：將自己的臉放到喜歡的電影或遊戲角色上，創作個人化內容。

+ 教育示範：用於教學示範，例如模擬歷史人物演講等。

+ 社群媒體互動：製作有趣的換臉短片，增加社交互動。

# 實際換臉成果

+ 要換臉的影片

https://github.com/user-attachments/assets/d48b7b2c-a0b0-4eb7-886d-4b3847a9730c

+ 要換進去影片的照片

![4FBEE21F-6758-4B40-B9B9-06434A646975](https://github.com/user-attachments/assets/ab667270-d623-4f1c-a350-e3e1819a3b82)

+ 換完的成品

https://github.com/user-attachments/assets/316e8767-f4cd-4f9a-b9cf-717f1b36af9a

+ 照片、影片均經過本人同意，但影片結果可能是臉型、動作不相像的緣故，所以效果沒有很好

# 總結

+ 因為roop版本跟google cloab現在的版本不相容，所以在一開始做的時候一直出現錯誤。
+ 幾乎整個過程一直在試錯，我們依靠ai的幫忙完成修補版本不同的錯誤，儘管如此也花上近3個小時的時間，才完成整個換臉程序。
+ 補丁內容包刮修正 NumPy 2.x 的相容性錯誤、移除 Colab 伺服器端環境中不需要的 TensorFlow 資源限制代碼，及提供一鍵式部署，已經建立在github上。(https://github.com/kity2233466/roop-colab-fix/blob/main/fix_roop.py)

組員：11315022許華秦、11218109薛妤芸

