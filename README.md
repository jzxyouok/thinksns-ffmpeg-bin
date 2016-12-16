# thinksns-ffmpeg-bin
ThinkSNS程序中视频转码的ffmpeg运行文件拓展包。

# 用途
在ThinkSNS <= 4版本中，使用了ffmpeg对用户上传的视频进行mp4转码，默认可选，不转码，但是许多用户都不会装ffpmeg.

# 这包存在的意义
使用户在Linux环境下快捷方便的为ts安装ffmpeg（本包文件为bin文件，可以与其他版本共存）。

# 安装前的前置环境需求：
- 必须使Linux
- 环境中安装了composer工具
- （可选）推荐CentOS 6以上系统
- （可能需求）翻墙，搭梯子

# 安装步骤

1. 检查cli环境的php版本信息，必须要php5.3.12以上版本，可以运行
  ```shell
  php -v
  ```
  查看版本，如果提示不存在php命令，请自行安装php。如果是CentOS 7,可以直接运行
  ```shell
  yum install php-cli -y
  ```
  进行安装 CentOS < 7的yum默认仓库安装的php版本无法满足，你也可以编译安装php。

2. 检查composer，运行
  ```shell
  composer -V
  ```
  可查看composer信息，如果提示命令不存在，自己搜索“composer”关键词，按照官方说明安装。

3. 进入TS程序目录，这里我们拟定为`/web/thinksns`目录作为ts程序文件目录，后面都将使用这个目录地址，这个地址是这里 * 拟定 * 的地址，所以后续目录，替换为你的ts的真实地址。
  运行
  ```shell
  cd /web/thinksns
  ```
  进入TS目录。

4. 运行composer进行ffmpeg-bin Component依赖
  ```shell
  composer require medz/thinksns-ffmpeg-bin
  ```

5. 进入后台
  ![视频转码配置](/ffmpeg-config-1.png)
  在 * ffmpeg安装路径 * 栏输入`/web/thinksns/bin/ffmpeg/ffmpeg`点击下面的保存，即完成。

# 👏
✅完成了

# 更多
如果有windows版本的，环境联系我哟～谢谢～邮箱 `shiweidu@outlook.com`,也可以直接提交pr或者issues给我哟。
