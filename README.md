# 许宇杰｜嵌入式软件开发作品集

面向嵌入式软件开发、机器人与智能硬件岗位的个人工程作品集。页面以真实设备的控制、通信、视觉部署与整机联调过程为主线，用于项目讲解和秋招投递。

## 在线访问

- 作品集网站：[yuyuyj-zs.github.io](https://yuyuyj-zs.github.io/)
- PDF 简历：`assets/resume/许宇杰_嵌入式软件开发_2027届.pdf`。

## 项目概览

| 项目 | 工程重点 | 作品集内容 |
| --- | --- | --- |
| 途 S1 智能小车控制、AI 视觉与实时图传系统 | STM32F407、FreeRTOS、Modbus RTU、MAVLink、RV1106、RKNN、RTSP | 系统架构图、实车照片、气球检测、方向追踪及控制演示视频 |
| 基于 RK3566 Zero 3W 的视觉检测无人机平台 | 飞控与动力系统调试、MTF-01 光流、机载视觉端、图传、3D 打印结构 | 悬停与视觉检测演示、设备结构与检测画面 |
| 实验室环境监控与消毒系统 | STM32F103ZET6、ESP8266、多传感器、OneNET、远程控制 | 环境采集、云端上传与消毒联动的工程实践说明 |

## 作品集呈现方式

页面不把项目写成传统简历条目，而是按可讲解的工程 Case Study 组织：

```text
系统目标
→ 端到端架构
→ 实机照片与演示视频
→ 个人负责内容
→ 关键实现、问题定位与验证结果
```

其中，小车项目保留控制、视觉、图传和 Android 端的完整系统能力说明，同时明确个人负责需求拆解、硬件接入、环境配置、代码验证、部署、问题定位与整机联调。无人机项目明确视觉控制与自主控制算法由团队其他成员负责，个人承担硬件平台搭建、动力系统调试、光流接入、悬停验证、气球检测模型训练及整机联调。

## 工程实践范围

- **MCU / 控制：** C、STM32F1 / F4、FreeRTOS、HAL / CubeMX、UART、DMA、TIM / PWM、ADC、SPI、I²C
- **嵌入式 Linux / 通信：** RV1106、交叉编译、Makefile、Modbus RTU、MAVLink、SBUS、RTSP / RTP、UDP
- **视觉部署 / 调试：** YOLOv5、RKNN、RGA、示波器、逻辑分析仪、软硬件联调

项目开发中使用 AI 编程工具辅助完成部分代码生成与迭代；个人重点在于理解接口与系统、配置和修改代码、完成真实设备部署与端到端验证。

## 仓库结构

```text
.
├── index.html                    # 单文件静态作品集：HTML、CSS 与 JavaScript
├── assets/
│   ├── web/                      # 面向网页播放优化的视频与封面
│   ├── resume/                   # PDF 简历
│   ├── *.jpg / *.png             # 实机照片与系统架构图
│   └── *.mp4                     # 原始演示素材
└── .github/workflows/
    └── deploy-pages.yml          # GitHub Pages 自动部署
```

## 本地查看

本项目不依赖 Node.js 或构建环境。可直接双击打开 `index.html`，或在仓库根目录启动静态服务：

```bash
python -m http.server 4173
```

然后访问 `http://localhost:4173/`。

## 部署

推送至 `main` 分支后，GitHub Actions 会将静态页面自动部署到 GitHub Pages。线上页面与仓库内的 `index.html`、`assets/` 保持一致。

## 联系方式

- 邮箱：yuyujie04@qq.com
- 电话：138-5984-4355
