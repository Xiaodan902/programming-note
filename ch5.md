## CH5 函數
### 認識函數
#### 函數原型宣告
- 通常位於#Include與main()之間或也可放在main()函數中
- 若在為定義函數的情況下使用函數，C編譯器就會傳回為定義的錯誤
- 宣告函數之語法  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/45fe340c-8669-43a3-ab57-e6abe8a3aee5)
- ex：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/9ba31bbc-e153-4872-9b17-b715e33b2e16)
- 若函數不用傳回任何值或沒有任何參數傳遞，都可用void關鍵字形容
- ex：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/104e30ef-abe5-4eac-b4a4-2f590bec365a)
#### 定義函數主體
- 盡量使用有意義的名稱來命名
- 參數列需要同時填上資料型態和參數名稱
- 若此函數不需要傳入參數，則可在括號內指定void資料型態或省略成空白
- 最後的return回傳值須與函數型態相同
- 若函數宣告型態為void，最後的return可省略或只寫return後面不加回傳值    
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/3ec21d5d-32e3-46a2-a10c-2b5d18712cdd)
### 參數傳遞方式
- 可分為傳值呼叫(call by value)和傳址呼叫(call by address)
- 引數：又稱為實際參數，為我們實際呼叫函數時所提供的參數
- 參數：又稱為形式參數，為在函數主體或原型中所宣告的參數
#### 傳值呼叫
- 不會更動到原先主程式所呼叫的變數內容
- 為C/C++預設參數傳遞方式
- 宣告型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/2c40e51d-43c2-43fe-93a7-a9c768cac350)
- 呼叫型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/7e7d1dc2-cbf5-4fff-9559-8bfb38f440ea)
- ex：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/9841d9e3-e262-4501-8fa0-fbdba9ea239f)
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/9c4da013-5198-499f-8a8c-79cfea834eaa)
#### 傳址呼叫
- 在呼叫函數時，系統並沒有另外分配實際的位址給函數形式參數，而是將時實際參數傳遞給所對應的形式參數
- 進行取址時必須使用到"*"取值運算子和"&"取址運算子
  - 取值運算子(*)：可以取得變數在記憶體上所儲存的值
  - 取址運算子(&)：可以取得變數在記憶體上的位址
- 宣告型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/3b2548dc-9f2a-45e5-99a4-134adb78d9b9)
- 呼叫型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/54d61850-bf1f-4530-8d6c-61db2347ff5b)
- ex：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/be055d86-1282-4471-91c1-fbdf5757d16d)
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/c13a9b3d-c69d-4c12-b5aa-ecd2cebaa1ac)
#### 傳參考呼叫
- 只有C++才有的模式
- 類似傳址呼叫，但形式參數並不會另外配置記憶體存放實際參數傳入位址，而是直接把形式參數作為實際參數的一個別名(alias)
- 可以做到傳址呼叫的功能，並有傳值呼叫的簡便
- 宣告型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/08bfa51e-4a00-405b-8cc9-edd66aceb7ee)
- 呼叫型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/d4518bcf-c7e4-4cb5-96dd-f40877cbbf77)
- ex：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/cb177cb8-d9a6-4236-b5a2-88905b42dd8d)
![image](https://github.com/Xiaodan902/programming-note/assets/124233786/1fed3e73-6829-477b-aae1-0528702913fa)
#### 陣列參數傳遞
- 陣列名稱所存的值是陣列第一個元素的記憶體位址
- 可以直接利用傳址呼叫的方式將陣列指定給另一個函數
- 若在函數中改變了陣列內容，所呼叫主成是中的陣列內容也會改變
- 一維宣告型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/a8133ec5-d312-4c21-84fc-1968da3aa5b2)
- 一維呼叫型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/bc08cab7-bdda-4050-bd5e-bfe113de262c)
- 二維宣告型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/bbffa9fa-d518-48fc-ae4c-52ec455ad6a2)
- 二維呼叫型態：  
  ![image](https://github.com/Xiaodan902/programming-note/assets/124233786/9b9aa36f-5293-48ff-b8a5-8ced8f3f005c)











