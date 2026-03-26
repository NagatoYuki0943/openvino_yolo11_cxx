# openvino yolo 目标检测

参考 https://github.com/ultralytics/ultralytics/tree/main/examples/YOLOv8-OpenVINO-CPP-Inference

# 依赖

- opencv
- openvino
- eigen3 (目标追踪)

> 目标追踪使用了 [junhui-ng/ByteTrack-CPP: C++ implementation of ByteTrack algorithm](https://github.com/junhui-ng/ByteTrack-CPP) 项目源码


# 编译好的程序使用方式

例子

```sh
============================================================
OpenVINO YOLO C++ Demo help:
    for predict image, usage: ./rknn_yolo11_demo predict_image <model_config_path> <image_path>
    for predict video, usage: ./rknn_yolo11_demo predict_video <model_config_path> <video_path>
    for track video, usage: ./rknn_yolo11_demo track_video <model_config_path> <video_path>
============================================================

# for predict image, usage:
# 执行后会在执行目录生成 bus--predict.jpg
./main predict_image models/metadata.json images/bus.jpg

# for predict video, usage:
# 执行后会在执行目录生成 MOT16-08-raw--predict.mp4
./main predict_video models/metadata.json videos/MOT16-08-raw.mp4

# for track video, usage:
# 执行后会在执行目录生成 MOT16-08-raw--track.mp4
./main track_video models/metadata.json videos/MOT16-08-raw.mp4
```
