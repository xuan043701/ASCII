# ASCII Video Player

这是一个能够将视频转换为ASCII字符艺术并在终端中播放的Python程序。通过预处理视频并将其缓存到本地文件，可以流畅地在支持ANSI转义序列的终端中观看ASCII视频。

## 功能特点
- 将彩色视频帧转换成带颜色的ASCII字符。
- 支持视频帧的预计算和缓存，以提高播放性能。
- 在终端中控制视频播放速度。

## 依赖库
确保安装了以下Python库：
- blessed - 用于生成ANSI转义序列来着色文本输出。
- opencv-python(cv2) - 用来读取和处理视频文件。
- numpy- 提供对图像数据的操作支持。
- pickle- 用于序列化/反序列化ASCII帧数据至磁盘。

可以通过运行如下命令安装所需库：

pip install blessed opencv-python numpy


## 使用方法
1. 确保您的系统已正确配置好Python环境，并且已经安装了上述列出的所有依赖库。
2. 将要转换的视频放置于适当位置，并修改脚本中的`video_path`变量指向该视频。
3. 运行主程序：
 
   python ascii_video_player.py
 
4. 按下Ctrl+C可随时停止视频播放。

> 注意：请根据实际使用的终端窗口大小调整脚本中的width参数，以获得最佳显示效果。
> 每次在cmd窗口运行时都会删除缓存文件以重新写入
     ' 缓存文件 ascii_cache.pkl 已删除'
> 1. 导航到脚本目录：使用 'cd' 命令切换到包含 main.py 的目录。例如，如果你的脚本在' C:\Users\xuan0\PycharmProjects\PythonProject'目录下，你可以输入：

   cd C:\Users\xuan0\PycharmProjects\PythonProject

2. 运行脚本：在命令提示符中输入以下命令来运行你的脚本：

   python main.py
