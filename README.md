[![GitHub](https://img.shields.io/github/license/wukongdaily/DockerTarBuilder.svg?label=LICENSE&logo=github&logoColor=%20)](https://github.com/wukongdaily/DockerTarBuilder/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/wukongdaily/DockerTarBuilder.svg?style=flat&logo=appveyor&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/wukongdaily/DockerTarBuilder.svg?style=flat&logo=appveyor&label=Forks&logo=github) [![Github](https://img.shields.io/badge/RELEASE:DockerTarBuilder-123456?logo=github&logoColor=fff&labelColor=green&style=flat)](https://github.com/wukongdaily/DockerTarBuilder/releases) [![Bilibili](https://img.shields.io/badge/Bilibili-123456?logo=bilibili&logoColor=fff&labelColor=fb7299)](https://www.bilibili.com/video/BV1yyq6YREdF) 

## 🤔 这是什么？
[操作步骤](README_CN.md) | 简介 <br>
它是一个工作流。可快速构建指定架构/平台的单个或多个docker镜像 并存储在Artifact文件或Release文件

## 使用说明
在 Actions 中运行 **Docker Tar Builder** 工作流：
> `docker_images`：镜像名称，多个用逗号/空格分隔（支持中文逗号）<br>
> `platform`：`amd64` / `arm64` / `arm32` / `all`（`all` 会并行构建三种架构）<br>
> `output`：`release`（单文件需小于 2GB，超出的文件会自动改为 Artifact 上传）或 `artifact`<br>
> `retention_days`：Artifact 保留天数（1-90）<br>
> 工作流会先清理 Runner 磁盘（约多出 30GB 空间），并使用 pigz 多线程流式压缩，较大的镜像也能处理。

## 2024-12-09 新增功能：
> 增加了新的工作流<br>
> 可以将docker镜像转存到自己项目的Github Release文件里<br>

> [![Github](https://img.shields.io/badge/RELEASE:DockerTarBuilder-123456?logo=github&logoColor=fff&labelColor=green&style=for-the-badge)](https://github.com/wukongdaily/DockerTarBuilder/releases)<br>

> 如果Github Release文件下载缓慢 你可以在<br>         

> [![Github](https://img.shields.io/badge/国内加速站下载-FC7C0D?logo=github&logoColor=fff&labelColor=000&style=for-the-badge)](https://wkdaily.cpolar.top/archives/1)
 
## 教学视频
https://www.bilibili.com/video/BV1EZ421M7mL<br>
https://www.bilibili.com/video/BV1yyq6YREdF
## 解压工具
> Windows 上推荐使用7zip<br>
> macOS 推荐使用MacZip<br>
> Linux上推荐直接用tar 命令

## ❤️其它GitHub Action项目推荐🌟 （建议收藏）⬇️
- ### [一键生成run插件] 🆕
- https://github.com/wukongdaily/RunFilesBuilder<br>
- ### [一键构建自定义软件包大小的Immortalwrt] 🆕
- https://github.com/wukongdaily/AutoBuildImmortalWrt
- ### [OpenWrt/Armbian 安装器ISO] 🆕
- https://github.com/wukongdaily/armbian-installer
## 在哪里可以搜索或查询docker镜像的详细信息
### [查询镜像的详细信息 点击这里直达](https://docker.fxxk.dedyn.io/)
