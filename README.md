# yolov5-Object-Detection
训练项目文件夹格式：
VOCData——
        ——Annotations（标注文件.xml）
        ——dataSet_path（路径）
        ——images（训练图片）
        ——ImageSets（说明文件）
        ——labels（训练结果）
xml_to_yolo.py文件和split_train_val.py文件放置于项目文件夹下，主要用于转换文件格式等
detect.py文件替换yolov5中原本的detect.py文件
yolov5s.pt是预训练模型
yolov5s.yaml和myvoc.yaml是预训练模型的配置文件
best.pt是训练后得到最符合预期的模型权重

运行python detect.py  --weights best.pt --source path/ --save-txt进行测试
