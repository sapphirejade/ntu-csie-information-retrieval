# ntu-csie-information-retrieval

「資訊檢索與擷取」期末專題：[隱私保護與醫學數據標準化競賽：解碼臨床病例、讓數據說故事](https://codalab.lisn.upsaclay.fr/competitions/15425?secret_key=db7687a5-8fc7-4323-a94f-2cca2ac04d39)

## 資料夾
共分四個資料夾。
### src
程式碼所在。主要是以下三個檔案，其餘為階段實驗。
* [Preprocess_Single_Line.ipynb](/src/Preprocess_Single_Line.ipynb) 資料前處理
* [Postprocess_Single_Line.ipynb](/src/Postprocess_Single_Line.ipynb) 資料後處理
* [Pythia_70m.ipynb](/src/Pythia_70m.ipynb) 模型訓練

檔案在Windows、MacBook Pro M2、Google Colab環境下執行，但有幾點須注意。
* 針對Windows/MacBook Pro M2：須將Repository完整Clone，並在Repository中配置.venv或.conda環境。因為程式碼檔案讀寫是照Repository目錄相對路徑執行。
* 針對Google Colab：須將整個Repository放置到Google Drive，並在執行給予授權。因為Google Colab僅提供運行環境，資料無法永久保存在其虛擬機。

### res
資料集所在。主要是以下四個資料夾，其他是原始資料集壓縮檔。
* [Demo_Dataset](/res/Demo_Dataset/)：講師在課堂分享上所提供的資料集
* [First_Dataset](/res/First_Dataset/)：「子任務 1：病患隱私資訊擷取」資料集
* [Second_Dataset](/res/Second_Dataset/):「子任務 2：時間資訊正規化」資料集
* [opendid_test](/res/opendid_test/)：最終競賽資料集

### out
放置「前處理」、「模型訓練」、「後處理」之結果。
* [first_train_single_line.tsv](/out/first_train_single_line.tsv)：「子任務 1：病患隱私資訊擷取」資料集，前處理後之TSV
* [second_train_single_line.tsv](/out/second_train_single_line.tsv)：「子任務 2：時間資訊正規化」資料集，前處理後之TSV
* [merged_train_single_line.tsv](/out/merged_train_single_line.tsv)：前兩項子任務前處理後，合併所得之TSV
* [2023-12-02_13-30-31_answer.txt](/out/2023-12-02_13-30-31_answer.txt)：最終競賽，模型運算結果
* [2023-12-02_13-30-31_answer_post.txt](/out/2023-12-02_13-30-31_answer_post.txt)：最終競賽，模型運算&後處理之結果


### tutorial
開發過程所參考之網站資源範例。
