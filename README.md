# PVZ-Soudache

> Plants vs. Zombies - Soudache
> 植物大战僵尸 - Soudache，Godot 引擎自制同人项目

## 📖 项目介绍

PVZ-Soudache 是基于 **Godot Engine** 开发的《植物大战僵尸》同人游戏项目。
项目现阶段正在制作**主界面 / 选关 UI**，目前仅完成 UI 素材与场景搭建，尚未编写游戏交互逻辑脚本。
项目采用 Git  分支管理：`main` 作为稳定主干分支，`develop` 为集成开发分支，功能特性在独立分支开发（当前在 `index` 分支开发主界面）。

> ⚠️ 重要声明：本项目仅为个人业余同人创作，**非官方作品，不用于任何商业用途**。《植物大战僵尸》相关 IP 版权归原持有方所有。

## 🛠️ 开发环境

- 游戏引擎：Godot Engine
- 脚本语言：GDScript（后续实现游戏逻辑）
- 版本控制：Git + GitHub
- 资源格式：PNG 贴图、Godot 场景文件 `.tscn`、资源导入配置 `.import`

## 📂 目录结构（当前）

```
pvz-soudache/
├── .gitignore             # Git忽略文件配置
├── .editorconfig
├── .gitattributes
├── icon.svg
├── icon.svg.import
├── README.md
└── project.godot          # Godot项目主配置文件
```

## 🧩 分支规范

项目使用简化版 Git 分支管理：

表格

| 分支名       | 用途                             |
| --------- | ------------------------------ |
| `main`    | 稳定发布分支，存放可运行成品版本，禁止直接在此分支开发新功能 |
| `develop` | 开发集成分支，所有功能开发完成、测试后合并到此分支      |
| `index`   | 功能分支：主界面 UI 开发分支               |

> 开发流程：从 `develop` 新建功能分支 → 在功能分支开发、提交推送 → 开发完成后通过 PR 合并回 `develop`；
> 多个功能全部测试稳定后，再将 `develop` 合并到 `main`。

## ✅ 开发进度

- Godot 项目初始化，基础项目架构搭建
- 主界面（选关界面）UI 贴图资源导入
- index.tscn 场景搭建，界面元素布局
- 编写界面交互逻辑脚本
- 游戏核心玩法开发
- 关卡、植物、僵尸内容制作

## 🚀 如何运行项目

1. 克隆仓库到本地

```
git clone https://github.com/FengWenxi/PVZ-SDC.git
```

1. 打开 Godot Engine，导入项目
2. 在编辑器中打开场景 `scene/index.tscn`，预览主界面

## 📜 许可证

本项目为**非商业同人项目**：

- 项目内原创代码、自制美术资源仅用于个人学习与演示，禁止商用、二次分发。
- 《植物大战僵尸》相关 IP、原版美术素材版权归属原 EA/PopCap。

## 💡 开发备注

- 所有功能在独立分支开发，完成后通过 Pull Request 合并回 develop，保护 main 分支稳定。
- Godot 贴图对应的`.import`资源配置文件随项目一并提交，保证多人 / 多设备打开项目时资源配置一致。

