# 说明

基于 [Gifsicle](https://www.lcdf.org/gifsicle/man.html)，可批量「无损压缩」 GIF 图片的命令行工具。

> 无损压缩说明：仅对 GIF 做「透明度存储」和「移除每一帧的本地颜色表」处理，这两种处理对于实际表现是「几乎无损」的。前者也是网上各类 GIF 压缩工具的主要优化方向。

## 快速开始

全局安装

```shell
$ npm i https://github.com/tofrankie/gif-optimize.git -g
```

使用

```shell
$ gg <source-dir> -o <target-dir>
```

目前仅接受「输入」与「输出」两个参数，其中 `-o`、`--output` 表示输出目录，其余参数均表示输入目录（路径）。输入可以是目录、文件或者两者结合，若是目录，则会遍历目录下所有 GIF 文件（不含子目录）。

## 截图

![](./images/screenshot.png)

## 其他

⚠️ 注意，部分 GIF 经 Gifsicle 处理后，体积反而会变大，此时会将源文件原封不动地输出。
