# Simplest-FFmpeg-Video-Player
最简单的基于FFmpeg的视频播放器。

本程序实现了视频文件的解码和显示（支持HEVC，H.264，MPEG2等），本版本中使用SDL消息机制刷新视频画面。

相较于原程序，新增以下功能：

1. 可以提取并打印视频文件相关的信息
2. 窗口可以移动，可以调整大小
3. 按下空格键（SPACE）后暂停，再次按下空格后继续播放
4. 左Shift键控制显示彩色/黑白图像

若要实现脱离开发环境，在命令行下播放任意一个视频文件，则将代码：

```c
char filepath[] = "屌丝男士.mov";
```


修改为：


```c
char *filepath = argv[1];
```



修改后运行程序，在项目文件夹Debug下移入程序需要的dll文件和视频，在命令行输入：

```c
Simplest FFmpeg Player 屌丝男士.mov
```

即可播放视频。
