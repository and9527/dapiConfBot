# dapiConfBot
# 標題: 線上教室助理機器人
# 組員：馮文龍,詹德立,謝孟諺,翁宗民,高國原
# 提案
## Why(提案動機)?
> 線上多人互動教室或線上會議室已經有許多實際應用案例，然而許多控制介面仍然侷限於傳統的滑鼠控制，並不符合人類自然表達的方式，本組希望藉由機器學習識別影像串流中的手勢來發出控制指令，例如，靜音，取消靜音，切換投影片等，以協助**教室/會議管理者** 管理線上**虛擬教室/會議室**
## Who(分析結果的使用目標族群)?
> 1. 線上多人互動教室使用者或管理者
> 2. 線上會議室使用者或管理者
> 3. 特殊情境使用者如聾啞人士
## Where(分析的原始資料來源)?
> 1. 暫時先根據gesture.ai所提供的Node.js，試用其可行性
> 2. 尋找動作的資料(若無免費資料，可能自行收集)
## What(預計的分析結果)?
<ol>

*手勢*

![f]( https://www.fluentu.com/blog/chinese/wp-content/uploads/2017/11/chinese-gestures-e1512759046169.jpg    "hand" )

</ol>



| 助理機器人得到指令 | 左| 中| 右|
| :-------- | :--------|:--------|:--------|
| 使用者的手勢 | 發言權切換至使用者 | 發言權切換至主講者 | 告知主講者，使用者提出問題 |
|主講者的手勢 |切換投影片 | 靜音並且發言權切換至主講者 | 取消靜音 |

## 分析方法:

A conference bot implementation based on Gesture.ai or Microsoft/Google Vision API

## 備註：
宗民：(有想到會再改)

一開始是思考如果可以完全如同未來外星科技一樣(電影那種)，你推拉滑移，舉手，就會跟直覺上的用法一樣。例如舉手就是發問、往左撥就是換頁、手指著特定位置就可以開啟特定東西，喊特定東西特定東西就出來。

但這樣不實際

mac dafault的鍵盤右鍵點擊法也不是真的依循舊有的直覺(雙指點擊) 因此很多事情只要習慣就好

大概看到了這個

http://research.ibm.com/dvsgesture/

已經有不少gesture AI 的database

雖然還沒有細看 但我猜如果把對應關係轉換 應該就可以了
只要直覺上差異不要過大

初期可以先右邊有個可以拉開關掉的伸縮表 裡面有對應的動作跟效果


另一點些想到的是 如果是線上互動平台

除了 主要對話的人臉 其他都是可以變動的

像是可能會出現人臨時離開  複數人同時干擾

複數人可能需要定位就只看一個人 也就是起始那個人
人會分神打瞌睡 可以比照另一組有提過的
開車分神用手機提醒那個 
如果有分神會有訊息提醒

但人離開的話 不會被判定是打瞌睡 
但系統會計時之類的?

但這些都是後話
------------------------

我想
先思考Mac切換視窗 滑鼠右鍵等等
似直覺動作 只要稍微學習 就可以熟悉的半對應介面

處理這種為優先 細部更接近直覺的對應等有data再弄
