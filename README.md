# Ting Reader - 1Panel 应用包

本项目提供了 [Ting Reader](https://github.com/dqsq2e2/ting-reader) 在 [1Panel](https://1panel.cn/) 面板上的应用适配包。

## 目录结构

```text
.
├── ting-reader/       # 1Panel 应用包目录
│   ├── 1.0.10/        # 应用版本目录
│   ├── data.yml       # 应用元数据
│   ├── logo.png       # 应用图标
│   └── README.md      # 应用说明
└── ...
```

## 使用方法

### 方法一：直接上传（推荐）

1.  下载本项目 Release 页面最新发布的 `ting-reader-1panel.zip` 压缩包。
2.  解压压缩包，获得 `ting-reader` 文件夹。
3.  将 `ting-reader` 文件夹上传到 1Panel 服务器的本地应用目录：
    *   默认路径：`/opt/1panel/resource/apps/local/`
    *   上传后路径应为：`/opt/1panel/resource/apps/local/ting-reader/`
4.  登录 1Panel 面板，进入「应用商店」。
5.  点击右上角的「更多」->「同步本地应用」。
6.  在侧边栏选择「本地应用」，找到 **Ting Reader** 点击安装即可。

### 方法二：Git Clone

如果你熟悉命令行，也可以直接在服务器上操作：

```bash
cd /opt/1panel/resource/apps/local/
git clone https://github.com/dqsq2e2/ting-reader-1panel.git temp_repo
mv temp_repo/ting-reader ./
rm -rf temp_repo
# 然后在面板中同步本地应用并安装
```
