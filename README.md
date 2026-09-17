<div align="center">
  <h1>SPPModules</h1>
  <p>🚀 基于 YOLO 的 SPP (空间金字塔池化) 模块复现与改进合集</p>

  <!-- 徽章 -->
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue.svg" alt="Python">
  <img src="https://img.shields.io/badge/PyTorch-1.10%2B-red.svg" alt="PyTorch">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
</div>

---

## 项目简介

本项目实现了多种注意力机制与池化模块的变体，用于提升目标检测模型的性能。所有模块基于 PyTorch 编写，旨在捕获多尺度上下文信息并增强特征建模能力。

## 模块说明

| 模块文件 | 模块名称 | 简要说明 |
| :---: | :---: | :--- |
| `ASPP.py` | ASPP | 空洞空间金字塔池化，通过不同膨胀率的空洞卷积捕获多尺度上下文信息 |
| `DBSPPF.py` | DBSPPF | 密集连接空间金字塔池化，增强特征复用与梯度流动 |
| `PMHSA.py` | PMHSA | 并行多头自注意力模块，用于增强全局特征建模能力 |
| `SE_SPPF.py` | SE_SPPF | 引入 SE 通道注意力的 SPPF 模块 |
| `SPPF_LSKA.py` | SPPF_LSKA | 结合大核可分离注意力的 SPPF 模块，在降低计算量的同时扩大感受野 |

## 环境依赖

* Python 3.8+
* PyTorch 1.10+
* 其他依赖请根据实际情况安装（如 `numpy`, `torchvision` 等）