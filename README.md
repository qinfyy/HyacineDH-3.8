# HyacineDH

**__项目已经[迁移](https://github.com/DBKAHHK/HyacineDH-Core)！__**

<p align="center">
<a href="https://visualstudio.com"><img src="https://img.shields.io/badge/Visual%20Studio-000000.svg?style=for-the-badge&logo=visual-studio&logoColor=white" /></a>
<a href="https://dotnet.microsoft.com/"><img src="https://img.shields.io/badge/.NET-000000.svg?style=for-the-badge&logo=.NET&logoColor=white" /></a>
<a href="https://www.gnu.org/"><img src="https://img.shields.io/badge/GNU-000000.svg?style=for-the-badge&logo=GNU&logoColor=white" /></a>
</p>
<p align="center">
  <a href="https://discord.gg/AjBSd5rP5K"><img src="https://img.shields.io/badge/Discord%20Server-000000.svg?style=for-the-badge&logo=Discord&logoColor=white" /></a>
</p>

[EN](docs/README_en-US.md) | [簡中](README.md) | [繁中](docs/README_zh-CN.md) | [JP](docs/README_ja-JP.md)

## 📖介绍
特征：支持游戏的3.8版本。

## 💡功能

- [√] **商店**
- [√] **编队**
- [√] **抽卡** - 自定义概率
- [√] **战斗** - 场景技能中有一些错误
- [√] **场景** - 行走模拟器、交互逻辑、实体加载
- [√] **基本的角色培养** - 应该没问题
- [√] ~~**任务**~~ - 并不支持
- [√] **朋友** - 支持
- [√] **忘却之庭 & 虚构叙事 & 末日幻影** - 异相仲裁正在开发中
- [√] ~~**模拟宇宙 & 黄金机械**~~ - 无法游玩: )
- [√] **成就** - 可用

- [ ] **更多**  - Coming soon...

## 🍗使用&安装

### 快速启动

1. 在 [仓库发布页](https://github.com/DBKAHHK/HyacineDH/releases/tag/v1.0) 下载可执行文件
2. 打开下载完成的 `HyacineDH.zip` 解压至任意文件夹 __*应当使用英文路径*__
3. 提示：内置资源缓存。你可以直接启动服务器，而不必下载Resources

> (可选) 在源代码的WebServer文件夹中下载 `certificate.p12` 使得以HTTPS模式启动 ~~增加了一点没用的安全性~~: )

3. 运行GameServer.exe
4. 运行代理 启动游戏 链接，享受！

### 构建

DanhengServer 使用 .NET Framework 构建

**前置：**

- [.NET](https://dotnet.microsoft.com/)
- [Git](https://git-scm.com/downloads)

##### Windows

```shell
git clone --recurse-submodules https://github.com/DBKAHHK/HyacineDH.git
cd .\HyacineDH
.\dotnet build # 编译
```
##### Linux （Ubuntu 20.04）
```shell
# 添加 Microsoft 包存储库
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb
rm packages-microsoft-prod.deb

# 安装 .NET SDK
sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-8.0
```

- 编译并运行环境
```shell
git clone --recurse-submodules https://github.com/DBKAHHK/HyacineDH.git
cd DanhengServer
.\dotnet build # 编译
./Gameserver
```
**向 Microsoft 显示其他系统版本**
- [微软教程](https://dotnet.microsoft.com/zh-cn/download/dotnet/thank-you/sdk-8.0.204-linux-x64-binaries)

## ❓帮助

- 支持安卓系统
- 发现问题，请进入我们的服务器或提交issue反馈

## ❕️故障排除

获取常见问题的解决方案或寻求帮助，请加入[我们的Discord服务器](https://discord.gg/AjBSd5rP5K)

## 🙌鸣谢

- Weedwacker - 提供 kcp 实现
- [SqlSugar](https://github.com/donet5/SqlSugar) - 提供 ORM
- [LunarCore](https://github.com/Melledy/LunarCore) - 一些数据结构和算法
- C1enQwq - 提供一些代码，还有原型文件
- StopWuyu及DanhengServer的其它开发者 - 本项目是[DanhengServer-OpenSource](https://github.com/EggLinks/DanhengServer-OpenSource)的fork仓库
