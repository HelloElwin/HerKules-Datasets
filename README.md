# HerkulesDataset

Robot detection dataset by HKU Hercules

## Convert the original format to coco format

[raw2coco.py](https://github.com/HelloElwin/HerkulesDataset/blob/coco_test/raw2coco.py)

### 文件结构：
```
HerDataset1.0/
    train/
        <filename0>.png
        <filename1>.png
        ...
    train.json
    val/
        <filename0>.png
        <filename1>.png
        ...
    val.json
```

### 关于标签

将原有的中文标签转成了英文，对照如下表。

| 中文        | English     |
| ----------- | ----------- |
| 机器人      | RobotBody   |
| 装甲板      | RobotArmor  |

`RobotBody`与`RobotArmor`都被划为了`Robot`的子标签以便后期添加障碍物等标签。
