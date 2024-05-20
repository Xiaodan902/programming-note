## CH3 流程控制結構
### 選擇結構
#### if,if-else,if-else if-else 指令
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/190d3f92-cf73-47ff-9fd7-26a8cfef79e7)
- 條件式內不必加分號
- 指令超過兩行必要用大括號
- else if後面要接條件式
- else 後面不用加條件式
- 頭一個為if
- 中間皆用else if
- 最後用一個else
- else if和else皆不是必要存在
#### switch指令
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/dc26b76b-6bab-4eb7-abf4-da4c70033445)
- 條件運算式可為一個變數或一個運算式
- switch下面所包含的程式需用大括號
- case 數值後面需用冒號
- 若程式敘述只有一個指令可以直接放在逗號後面，不必換行
- default 的作用像else一樣可加可不加

### 迴圈結構
#### for迴圈
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/bf738211-19e4-44f8-9dd3-2edb76ef8455)
- 為前測試型迴圈
- for後面的3個運算式中，一定要有設定跳離迴圈的條件及控制變數的遞增遞減值，否則會變成無限迴圈
- 3個運算式以分號做為區隔
#### 巢狀for迴圈
- 意思是for迴圈裡還有for迴圈
- 先執行最內圈的程式，再往外執行
#### while 迴圈
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/014bdf3b-61a9-4cc2-8c31-c3186c577eb7)
- 為前測試迴圈
- 條件判斷式相對於for迴圈有更廣的方向可以使用，但while需自行加入控制變數起始值旱地增減運算式，否則會變成無限迴圈
#### do-while迴圈
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/14056f9a-20a6-495e-b984-41d7f05963f2)  
- do while迴圈與while迴圈相似
- 為後測試迴圈
- 大括號內需要先有一個冒號
- 最後的while條件式後要加分號

### 流程控制指令
#### break指令
- 用途為跳離離break最近的迴圈
- 多半會配合if作使用
#### continue指令
- 用途為跳過該迴圈剩下的指令，將控制權回到迴圈開始處
- 並未跳離該迴圈
