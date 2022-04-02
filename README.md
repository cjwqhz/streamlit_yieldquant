# yoloV5ToStreamlit

#### 介绍
向streamlit移植YoloV5

#### 环境
python3.8
windowns10
pycharm

#### 使用说明

1.  将下载的zip包进行解压
2.  安装 streamlit

```
pip install streamlit
```
2.  cd 到 /yolo/下运行

```
pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple

```

3.  cmd 到main.py文件夹下
4.  运行命令

```
streamlit run main.py
```



#### 使用说明

1.  webFunction/indexFunction.py 文件中34，42行设置为自己的文件路径即可
2.  若想使用自己的权重文件
webFunction/indexFunction.py 文件中20行，添加如下属性即可
weightPath='weights/你的权重文件'（请将权重文件放入weights文件夹下）
3.  本项目是不存储检测后的文件和待检测文件，在检测完毕后会自动删除。
若想存储，修改webFunction/indexFunction.py中
对以下内容注释即可
remove_file(vs_name)
remove_dir(os.path.dirname(de_dir))
4.  若想对输出路径进行更改
webFunction/indexFunction.py 文件中20行，添加如下属性即可
savePath='你想存储的位置'（默认为：runs/detect）

#### 参与贡献

1.  https://github.com/ultralytics/yolov5
2.  https://docs.streamlit.io/
3.  https://blog.csdn.net/weixin_46234681/article/details/123194323
