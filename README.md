# AndroidDebugHelper
python 编写的用于辅助安卓调试apk的 adb / jdb 命令快捷调用脚本。

> 建议安装 termcolor 以获得更好的输出效果 (也就那样)
> `pip install termcolor`

```bash 
usage: python O:\HackTools\Android\AndroidDebugHelper\apkDebugHelper.py 
[-h] [-a [ANDROIDSERVER]] [-j [JDB]] [-i]
[-ia] [-k [KILLANDROIDSERVER]] [-p PATH] [-l]

optional arguments:
  -h, --help            show this help message and exit
  -a [ANDROIDSERVER], --androidServer [ANDROIDSERVER]
                        传入androidServer端口,开启androidServer,默认端口为23946。
  -j [JDB], --jdb [JDB]
                        传入jdb调试端口,链接jdb调试,默认为8700。
  -i, --apkInfo         获取apk信息,使用-p传入路径
  -ia, --installApk     覆盖安装apk,使用-p传入路径
  -k [KILLANDROIDSERVER], --killAndroidServer [KILLANDROIDSERVER]
                        关闭本程序传入的android_server。
  -p PATH, --path PATH  传入路径，用于查询信息或者调试apk
  -l, --log             打印将要执行的命令
```

可以单独使用 `-p` 参数并给到 apk 目录
以自动安装 apk , 启动 ands , 端口转发 , 等待启动jdb等操作

功能均可单独调用，以方便分步操作。
