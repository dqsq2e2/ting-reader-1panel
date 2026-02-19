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

### 一键安装命令（推荐）

通过 SSH 连接到您的服务器，直接执行以下命令即可快速安装：

```bash
# 进入 1Panel 本地应用目录
cd /opt/1panel/resource/apps/local/

# 下载最新的应用包
wget https://github.com/dqsq2e2/ting-reader-1panel/releases/download/latest/ting-reader-1panel.zip

# 解压应用包
unzip -o ting-reader-1panel.zip

# 删除压缩包
rm ting-reader-1panel.zip

# 设置权限（可选，防止权限问题）
chown -R root:root ting-reader/
```

### 安装步骤

1.  执行上述命令后。
2.  登录 1Panel 面板，进入「应用商店」。
3.  点击右上角的「更多」->「同步本地应用」。
4.  在侧边栏选择「本地应用」，找到 **Ting Reader** 点击安装即可。

## 开发与维护

本项目包含自动打包工作流。当 `ting-reader` 目录下的文件发生变更时，GitHub Actions 会自动触发打包，并发布到 `latest` 标签的 Release 中。
