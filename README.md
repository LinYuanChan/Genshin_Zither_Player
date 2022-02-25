# Genshin_Zither_Player
An auto zither player for Genshin Impact Winows Version,support midi files
Based on [pyautogui](https://github.com/asweigart/pyautogui) and [mido](https://github.com/mido/mido)

---
## TODO
- 播放/暂停/终止
- 制谱
----
# 原神自动弹琴脚本
这是一个支持在Windows端自动读取`midi`文件并演奏的原神弹琴脚本，基于[pyautogui](https://github.com/asweigart/pyautogui) 和 [mido](https://github.com/mido/mido)开发


## 安装使用
安装最新版本[Python](https://www.python.org/downloads/)并将其加入环境变量

解压release界面下载的压缩包.

### 使用步骤
打开原神, 进入弹琴界面, 最小化游戏窗口

打开`Genshin Zither Player`, **授予管理员权限**, 选择演奏曲目,演奏速度和升降调, 点击`Play`按钮并在等待时间内迅速打开最小化的原神游戏窗口, 等待时间过后即可开始演奏

如需暂停演奏请按`Win`+`L`

### 导入自定义midi

将midi文件放在`midi_repo`文件夹内, 打开脚本即可正常加载演奏

### 自动升降调/midi自适应功能

无需额外操作

由于原神琴键的限制，仅支持C大调音阶内三个八度的音符（即只能弹钢琴白键上的音符），因此许多原调的midi文件将不适用，使用本脚本可以解决这一问题，当选择了不是C大调/A小调的midi文件时，本脚本会尝试将其转调为Cmajor并演奏，对于市面上的流行歌曲成功率极高，只需要在选择升降调时按对应操作即可