# AI反诈项目 README

## 项目简介

在人工智能技术飞速发展的今天，电信诈骗和网络诈骗手段日益高明，特别是AI换脸和拟声技术的应用，使得诈骗行为更加隐蔽。为应对这一挑战，我们推出了“AI反诈”项目，利用AI技术实时识别和预防诈骗行为，保护人们的财产和人身安全。

## 产品功能

- **诈骗消息分析**：输入涉及转账、汇款、中奖等相关信息的短信或邮件文本，AI将帮助分析信息的真伪并给出处理建议。
- **合成人脸分析**：上传人像图片（如视频聊天截屏），AI将分析图片中人脸为AI合成的可能性，并给出分析的详细结果。
- **合成人声分析**：对比两段声音的声纹来分辨声音是否为本人。

## 应用价值

本项目旨在帮助用户远离诈骗，通过技术手段提升诈骗识别的准确性，为构建一个更安全的网络环境做出贡献。

## 技术方案

- 利用**RAG**技术强化大模型对诈骗信息的识别。
- 训练模型识别通过AI合成的人脸图片。
- 利用**声纹技术**，分析输入的两段音频是否为同一个人。

## 快速启动

本项目支持的python环境需在3.10以内，建议使用python3.9.19

要本地运行AI反诈项目，请按照以下步骤操作：

1. 安装依赖项：
   ```bash
   Pip install -r requirements.txt
   #运行在GPU环境则安装对应版本torch
   pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
   ```

2. 运行应用程序：
   ```bash
   python app.py
   ```

3. 运行Web界面（使用Streamlit）：
   ```bash
   streamlit run website.py
   ```

## 部署

- 初期计划将系统部署在云端，以便于快速访问和使用。
- 未来考虑本地部署，以增强隐私保护。

## 贡献
本项目由DataWhale夏令营第四期“天下无诈”组协作开发。
欢迎对本项目做出贡献，无论是代码、文档、还是提出宝贵的意见。


---

感谢您对AI反诈项目的关注和支持，让我们共同努力，打造一个更安全的网络世界。
