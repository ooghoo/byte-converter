# 字节换算 · Byte Converter

一个极简、零依赖的在线字节单位换算小工具。从百度搜索结果页的换算器单独抽出，去掉了所有无关的搜索列表与热搜，只保留纯粹的换算功能。

## ✨ 功能特性

- **实时换算**：输入数值即出结果，无需点击按钮
- **完整单位**：`bit` / `B` / `KB` / `MB` / `GB` / `TB` / `PB` / `EB` / `ZB` / `YB`
- **双规则切换**：
  - **Windows**：二进制进制，`1 KB = 1024 B`
  - **Mac**：十进制 SI 进制，`1 KB = 1000 B`
  - `1 Byte = 8 bit`，bit 始终不受进制影响
- **默认展开到 TB**，更大的单位（PB / EB / ZB / YB）折叠在「展开更多单位」下，点按展开
- **结果保留 2 位小数**（极小值自动切换科学计数法，避免被吞成 `0.00`）
- **一键复制**：每行结果悬停即出现复制按钮
- **单文件、纯静态、零第三方依赖**，离线也能用

## 🔗 在线使用

https://ooghoo.github.io/byte-converter/

## 🖥 本地使用

直接双击 `index.html` 用浏览器打开即可，无需服务器、无需联网。

## 🛠 技术说明

- 纯 HTML + CSS + 原生 JavaScript，全部内容在单个 `index.html` 中
- 以 **Byte** 为基准单位，按进制幂次动态换算
- 默认输入单位：**字节 (B)**

## 📦 自行部署

本项目通过 GitHub Pages 托管（`main` 分支根目录）。若需自行修改并部署：

```bash
git clone https://github.com/ooghoo/byte-converter.git
cd byte-converter
# 编辑 index.html
git add index.html
git commit -m "update"
git push
```

推送后 GitHub Pages 会自动重新构建。

---

纯工具，无追踪、无广告。
