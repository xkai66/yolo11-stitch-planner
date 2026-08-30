# yolo11-stitch-planner

YOLO11n 玉米杂草检测的 a+b+c 缝合规划页。

## 本地预览

在本目录运行：

```powershell
python -m http.server 8787
```

浏览器打开 `http://127.0.0.1:8787/`。表单保存到浏览器 `localStorage`；点击“下载 plan.json”后，文件可作为后续自动缝合脚本输入。

## 重要边界

当前训练入口 `C:\Users\xkai2\Desktop\训练集\yolov11\train.py` 还没有 `--stitch` 解析器。网页导出的 `train-stitch-config.json` 是定版后的接口草案，不代表当前训练脚本已支持该命令。

参数量/GFLOPs中标记“估算”的数值只用于筛选，最终须用 YOLO11n 实际构建、forward 和端侧测速结果替换。

完整方案见 [缝合计划-v0.1.md](./缝合计划-v0.1.md)。
