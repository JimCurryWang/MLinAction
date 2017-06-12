# MLinAction
Several Machine Learning Algorithm code with Python :blush:  
index: `Machine Learning` `Algorithm` `KNN` `SVM` 

## kNN: k Nearest Neighbors
    Input:      inX: vector to compare to existing dataset (1xN)  
                dataSet: size m data set of known vectors (NxM)  
                labels: data set labels (1xM vector)  
                k: number of neighbors to use for comparison (should be an odd number)  
            
    Output:     the most popular class label  

## SVM : support vector machine
`svm` `kernel` `空間轉換` `Seperating hyperplane` `SMO` 

基於序列最小優化算法（Sequential Optimization,SMO）   
    - 優點：**泛化誤差**（Generalization error）低  
    - 缺點：對**參數**的調節和 **核函數(kernel)** 的選擇敏感
    
   svm的優點在於能對數據進行高效分類，  
   如果支撐向量太少，就可能得到一個差的決策分界  
   如果支撐向量太多，也就是相當每次都利用整個數據及進行分類，那就等同於KNN。  
>
   - **SMO算法**：該算法通過每次只優化2個alpha值，來加快SVM的訓練速度。  
>
   - **Kernel** : 可以將數據從一個低維空間（有時為非線性數據）映射到一個高維空間，  
  可以將一個低維空間的非線性轉換成高維空間下的線性問題解決。   
>   
   - **Support Vector** : 離分割超平面(Seperating hyperplane)最近的點，  
  最大化支撐向量到分割超平面的距離 尋找最大間隔 找到該問題的優化求解，  
  if 數據點離決策邊界越遠，其最後的預測越可信，越能將兩群資料分開。
             
    
            

## Kmeans : 
    基於二分K-均值法（bisecting K-means）   
    - 優點：容易實現  
    - 缺點：在大規模數據下**收斂速度慢**，計算量大，且可能收斂到**局部最小值**
    
    隨機確定確定k初始點作為值心





## 備註：
####監督學習-分類(supervised learning):  
    需要知道目標值，簡單說知道數據在尋找什麼，訓練樣本要有標記。  
    給定輸入樣本進入模型，從中計算出該樣本的可能結果。  
####無監督學習-聚類(unsupervised learning)：  
    無需知道搜尋的目標，只需從算法程序中得到數據共同特徵。  
		  
>聚類分析試圖將相似對象歸入同一cluster，不相似歸到不同cluster。  
  簡單來說，分類的目標事先已知，已經知道我丟東西進去會大概得到哪幾種結果，  
  而聚類不一樣，其類別事前沒有預先定義，跑出來才會知道，  
  但是可以事前決定我要將資料集分成幾個群。

    
####泛化誤差（Generalization error）:  
>機器學習實驗過程，是我們希望通過訓練集能夠學習出在新樣本（測試集）上也表現良好的學習期（模型）。  
    我們常用「錯誤率」（error rate）或「精度」（accuracy）來量化模型的好壞程度，其中錯誤率 = 1 - 精度。    
    一般地，我們用「誤差」表示學習器的實際預測輸出與樣本的真是輸出之間的差異，在訓練集上的誤差稱為「訓練誤差」，  
    在新樣本（測試集）上的誤差稱為「泛化誤差」。  
    顯然地，我們希望「訓練誤差」和「泛化誤差」都儘可能的小。  
    這就需要權衡，從而引發了機器學習中最難解決的重大問題——過擬合（overfitting）和欠擬合（underfitting）。  
    原文網址：[https://kknews.cc/zh-tw/news/85bebbn.html]
    
    
    
