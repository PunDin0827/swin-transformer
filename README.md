1.下載好數據集，默認使用的是花分類數據集，下載地址: https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz

2.在`train.py中將`--data-path`設置成解壓縮後的`flower_photos`文件夾絕對路徑

3.下載預訓練權重，在model.py文件中每個模型都有提供預訓練權重的下載地址，根据使用的模型下載對應的預訓練權重

4.在train.py中將--weights參數設置成下載好的預訓練權重路徑

5.設置好數據集的路徑--data-path以及預訓練權重的路徑--weights就能使用train.py開始訓練(訓練過程中自動生成class_indices.json文件)

6.在predict.py中導入和訓練中同樣的模型，並將model_weight_path設置成訓練好的模型權重路徑(默認保存在weights文件夾下)

7.在predict.py中將img_path設置成需要預測的圖片絕對路徑

8.設置好權重路徑model_weight_path和預測的圖片路徑img_path就能使用predict.py進行預測

9.如果要使用自己的數據，可依照花分類數據的文件結構進行擺放(即一個類別對應一個文件夾)，並將訓練以及預測中的num_classes設置成自己數據的類別數量
