<h1 align="center">CC2027MK2</h1>

<p align="center">
  用 DeepSeek Harness 把日常真正会用上的小工具一个一个做出来。<br>
  全部 <b>本地运行</b> —— 不联网、不登录、无云端、无遥测。
</p>

---

## 🖥 [OpenRec](https://github.com/CC2027MK2/OpenRec) · Windows 本地录屏

参考录屏软件的**本地能力**做的干净复刻，不联网也能用全套。

- 全屏 / 拖框区域 / 指定窗口 / 仅音频，麦克风与系统声实时混音
- 摄像头画中画、鼠标指针、REC 水印、倒计时、暂停续录、全局热键、托盘常驻
- 录制库、剪辑、损坏文件修复、白板标注、局域网扫码看片、磁盘空间保护

<sub>Python · PySide6 · FFmpeg</sub><br>
<a href="https://github.com/CC2027MK2/OpenRec/releases/latest"><img src="https://img.shields.io/github/v/release/CC2027MK2/OpenRec?label=release&color=2ea44f" alt="release"></a>
<img src="https://img.shields.io/github/license/CC2027MK2/OpenRec?label=license&color=blue" alt="license">
<img src="https://img.shields.io/badge/platform-Windows-0078d4" alt="platform">

## 📱 [NfcTapLink](https://github.com/CC2027MK2/NfcTapLink) · 一碰传

碰一下 NFC 标签，手机和电脑之间就传文件——全程局域网直连，不经过任何服务器。

- Android 客户端（Java）+ Windows 桌面端（Python / PySide6）
- 标签里只放设备 ID 与配对密钥的哈希；密钥只存在本机
- 双向挑战应答配对，传输加密 + HMAC + 时间窗防重放，局域网内走 HTTP

<sub>Java · Python · PySide6</sub><br>
<a href="https://github.com/CC2027MK2/NfcTapLink/releases/latest"><img src="https://img.shields.io/github/v/release/CC2027MK2/NfcTapLink?label=release&color=2ea44f" alt="release"></a>
<img src="https://img.shields.io/github/license/CC2027MK2/NfcTapLink?label=license&color=blue" alt="license">
<img src="https://img.shields.io/badge/platform-Android%20%2B%20Windows-3ddc84" alt="platform">

## ⌚ [dsh-watch-phone](https://github.com/CC2027MK2/dsh-watch-phone) · 手表 ↔ 手机

把本地 DSH 接到智能手表上：抬手按住说话，手机上跑推理，手表上听结果。

- HTTP 桥（`/chat` `/reset` `/stt` `/tts` `/exec` `/relay`），同网段自动发现
- 手表端 APK + 手机插件 + PC 桥；离线 STT/TTS，不把语音传到云上
- 以 npm 包发布，CI 走 Trusted Publishing（零 token）

<sub>JavaScript · Android · npm</sub><br>
<a href="https://www.npmjs.com/package/dsh-watch-phone"><img src="https://img.shields.io/npm/v/dsh-watch-phone?label=npm&color=cb3837" alt="npm"></a>
<a href="https://github.com/CC2027MK2/dsh-watch-phone"><img src="https://img.shields.io/github/license/CC2027MK2/dsh-watch-phone?label=license&color=blue" alt="license"></a>
<img src="https://img.shields.io/badge/platform-Wear%20OS%20%2B%20Android-3ddc84" alt="platform">

## 🔌 [rs485-bridge](https://github.com/CC2027MK2/rs485-bridge) · RS485 网络网关

把一台机器的 RS485 口变成全屋可用的 Modbus TCP / raw TCP / HTTP 接口，单文件，只依赖 pyserial。

- 三种模式：`modbus`(502) / `raw`(5000) / `http`(8080，带 token 与 IP 白名单)
- 半双工总线全局锁、帧超时与打包窗口可调，约 15–30 次事务/秒（9600bps）
- 自带 12 项协议自测 + 12 项安全回归，`socket://` 假从站，不需要真实硬件

<sub>Python · pyserial · Modbus RTU/TCP</sub><br>
<img src="https://img.shields.io/github/license/CC2027MK2/rs485-bridge?label=license&color=blue" alt="license">
<img src="https://img.shields.io/github/actions/workflow/status/CC2027MK2/rs485-bridge/selftest.yml?label=selftest" alt="selftest">
<img src="https://img.shields.io/badge/platform-Windows%20%2B%20Linux-6e7681" alt="platform">

---

## 关于这个账号

- 所有仓库都用 **MIT** 许可（`awesome-dsh-plugin` 是 fork，遵循上游 CC0-1.0）
- 没有账号体系、没有统计上报，工具默认只在本机干活
- 用得到就 fork，遇到问题直接开 issue
