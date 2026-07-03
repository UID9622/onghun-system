# 快速开始 · Getting Started

> DNA: `#龍芯⚡️2026-07-03-ONGHUN-GETTING-STARTED-v1.0`

---

## 第一步：理解龍魂

不要急着跑代码。先读三篇核心文档：

1. [追本溯源哲学](philosophy.md) — 为什么做这件事
2. [七因子行为密码学](seven-factor-cryptography.md) — 核心引擎
3. [系统架构](architecture.md) — 整体结构

---

## 第二步：准备环境

```bash
# 克隆本仓库
git clone https://github.com/UID9622/onghun-system.git
cd onghun-system

# 安装 CNSH 运行时（可选）
# 见 longhun-cnsh 技能文档

# 检查本地依赖
python3 --version  # >= 3.8
```

---

## 第三步：生成你的第一个 DNA 追溯码

```python
import hashlib
from datetime import datetime

content = "这是我的第一条龍魂宣言。"
timestamp = datetime.utcnow().isoformat()
source = "UID9622"

source_data = f"{content}:{timestamp}:{source}:#龍芯⚡️"
dna = "#龍芯⚡️" + hashlib.sha256(source_data.encode()).hexdigest()[:16]
print(dna)
```

---

## 第四步：阅读蓝图仓库

更多可运行的模板和示例在：

[https://github.com/UID9622/uid9622-open-blueprint](https://github.com/UID9622/uid9622-open-blueprint)

---

## 第五步：参与贡献

见 [CONTRIBUTING.md](../CONTRIBUTING.md)。

---

*开始很简单，坚持很难。龍魂是长跑。*
