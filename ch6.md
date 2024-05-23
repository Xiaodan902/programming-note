## CH6 指標
### 認識指標
- 宣告指標變數
- 多重指標
- 指標運算
- 指標與陣列的應用
- 指標與字串
### 認識指標
- 可以看作一種變數，址是只能儲存記憶體位址
- 只要透過&就可以求出變數所在位址  
  &變數;
- 一般情況下，並不會直接處理記憶體位址，因為變數就已經包括的記憶體位址的資訊，會直接告訴成是應該到記憶體中的何處取出數值
#### 宣告指標變數
- 指標是專門用來儲存記憶體位址、進行與位址相關的運算、指定給另一個變數
- 由於指標也是一種變數，命名規則與一班我們常用的變數相同
- 定義指標的資料型態、在資料型態後加上"*"再給予指標名稱，即可宣告一個指標變數
- 指標變數可設定出值為0或是NULL  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/2e512675-8a17-4827-a552-b1b8373f91d5)
- 在未指定其初始值時，指標所指向的記憶體位址是未知的，不可對其進行存取
- 要指定指標的值，可以使用&取址運算子鄉變數所指向的記憶體位址指定給指標  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/4686ff0d-544e-4ce4-b297-1630c6888d65)  
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/ed06ddc6-7fc3-454f-99b2-90e6fabee67b)
- 數值、變數、記憶體與指標間的關係  
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/8cc5aaa6-b553-4447-85c8-ab20bab8442b)
- 確定指標所指向的資料型態，就不能再更改
- 指標變數不能指向不同資料型態的指標變數
- 相同型態資料中可以重新設定所要指向目標
#### 多重指標
- 有到三重指標
- 其表示方法：*(指標) **(雙重指標) ***(三重指標)
#### 指標運算
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/446e97bb-2400-4349-b747-c4fb5924c933)
#### 指標與陣列的應用
- 可以把陣列名稱當成一種指標常數來運作
- 可以將指標變數指到陣列的起始位址，並間接就能藉由指標變數台存取陣列中的元素值  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/3b950b22-b7a9-4af3-b6f6-d1569767c057)
- 此時陣列名稱arr唯一指標常數，也是此陣列的起始位址
- 只要在陣列名稱上加1或透過運算子&取得該陣列元素德未指，就可表示移動一個陣列元素記憶體的位移量
- 直接存取陣列內的元素值  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/127fdf78-60f5-43ef-88ae-e398209e3a01)
-取得一維陣列  
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/6fed2c7c-eec6-4508-b670-41f43bab1526)
- 二維陣列具有兩個引索值  
  ex: int no[2][4];  
  可使用*(no+i)+j取得位址
- 可藉由指標變數指向二維陣列起始位址來取得陣列的所有元素值
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/6c2b4fff-0be8-49b5-a9a7-0e7f52a18bee)
#### 指標與字串
- 可以用以下宣告格式來宣告字串  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/ed98eb1b-004a-459d-8073-e58023a1697c)
- 好處為可以改變其值並加以運算










