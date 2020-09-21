dapm_route 是一个 Linux ALSA 音频通路调试工具，可以把所有音频控件的状态通过图画的形式展示出来，方便音频驱动开发人员定位问题。使用方法如下：

1. 安装 graphviz：`sudo apt-get install graphviz`
2. 在 Host 直接执行：`./dapm_debug_host.sh`
3. 图片生成位置：`./tmp/dapm_route.png`

dapm_route_active.sh 仅列举 active 状态的控件，效果如下：

![active_route_example](https://github.com/sepnic/dapm_route/blob/master/active_route_example.png)

dapm_route_all.sh 列举所有的控件，包括 active 和 inactive 的，因为控件比较多，所有每个 dapm 目录一张图片，效果如下：

![all_route_example](https://github.com/sepnic/dapm_route/blob/master/all_route_example.png)


