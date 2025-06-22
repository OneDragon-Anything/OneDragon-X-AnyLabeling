# 一条龙标注

## 安装

见 [官方文档](https://github.com/CVHub520/X-AnyLabeling/blob/main/docs/en/get_started.md)

注意安装的 `onnxruntime` 版本需要和一条龙中使用的版本一致，否则无法使用加载模型预测功能

## 使用

1. `python anylabeling/app.py` 运行
2. `打开文件夹` -> 选择某个数据集的根目录，例如 [ZZZ-LostVoidDet-Dataset](https://www.modelscope.cn/datasets/DoctorReid/ZZZ-LostVoidDet-Dataset)
3. `导入` -> `Upload Label Classes File` -> 选择数据集下 `X-AnyLabeling/classes.txt`
4. `文件` -> `更改输出目录` -> 选择数据集下 `X-AnyLabeling/annotation`
5. 正常标注导出

### 使用已有模型标注

1. 复制数据集目录下 `X-AnyLabeling/onnx.example.yaml` 重命名 `onnx.yaml`
2. 修改 `onnx.yaml` 中的 `model_path`，指向当前最新的 onnx模型
3. 在X-AnyLabeling应用中加载自定义模型，选择 `onnx.yaml`