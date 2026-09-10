# LC-notes

> 计算语言学（Advanced Computational Linguistics）与 LLM 的学习笔记 —— 7 张**可交互思维导图**。

每一份笔记都是一个自包含的 HTML 思维导图（样式、字体、图片全部内嵌），支持**点击节点折叠 / 展开**，并带公式排版（KaTeX）。

---

## ⚡ 在线阅读（推荐）

启用 GitHub Pages 后，直接点下面的链接就能看到渲染好的思维导图：

**<https://mingxuanjin.github.io/LC-notes/>**

> 首次使用需要先开启 Pages，只需做一次 —— 见下方「🚀 开启 GitHub Pages」。
> 如果链接还打不开，先用下方「🌐 即时预览」里的 htmlpreview 顶上。

---

## 📖 目录

| # | 笔记 | 主要内容 | 在线阅读 | 源码 |
|---|------|---------|---------|------|
| 01 | **WSD** · 词义消歧 | 动机与历史 · 有监督 / 半监督 / 无监督方法 · 知识驱动（Lesk、选择偏好）· 评测框架 · 应用 | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/01-wsd.html) | [源码](advanced-cl-and-llm/01-wsd.html) |
| 02 | **Embeddings** · 词表示与 LLM 基础 | 显式→隐式范式 · VSM 构建 · 图嵌入 / 义项嵌入 · 上下文嵌入 · Transformer · 预训练 · 知识注入 · 提示工程 · 句嵌入 | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/02-embeddings.html) | [源码](advanced-cl-and-llm/02-embeddings.html) |
| 03 | **DS** · 分布语义学 | 核心定义与分布假设 · 四大理论支柱 · 5 步流水线 · 共现矩阵与加权（PMI/PPMI）· 相似度度量 · DSM 分类 · 神经网络模型 · 评测 | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/03-distributional-semantics.html) | [源码](advanced-cl-and-llm/03-distributional-semantics.html) |
| 04 | **Glossary** · 术语表 | 计算机与算法基础 · AI 分类 · 机器学习范式 · 神经网络与深度学习 · 向量语义 · LLM 架构与机制 · 训练与能力 · 对齐与安全 · 三大流派 | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/04-glossary.html) | [源码](advanced-cl-and-llm/04-glossary.html) |
| 05 | **AR & CR** · 回指与共指消解 | 核心术语 · AR vs. CR · 指代类型（零回指、指示词、预设、分裂先行语、后指、桥接）· 消解约束 · 数据集 · 算法与工具 | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/05-anaphora-coreference.html) | [源码](advanced-cl-and-llm/05-anaphora-coreference.html) |
| 06 | **NER** · 命名实体识别 | 命名实体的定义与来源 · 实体类型 · 学习方法（有监督 / 半监督 / 无监督）· 特征 · 评测与错误类型（MUC 指标） | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/06-ner.html) | [源码](advanced-cl-and-llm/06-ner.html) |
| 07 | **LLOD** · 语言关联开放数据 | FAIR 原则 · Linked Data 与语义网 · RDF / RDFS · 互操作性与 LLOD 云 · Ontolex-lemon 与元数据 · OLiA · 数据发布生命周期 · SPARQL | [打开 →](https://mingxuanjin.github.io/LC-notes/advanced-cl-and-llm/07-llod.html) | [源码](advanced-cl-and-llm/07-llod.html) |

> 「源码」链接指向仓库里的 `.html` 文件。**GitHub 会把 `.html` 当纯文本显示源码，这是它本来的行为**，所以要看渲染效果请用「在线阅读」或下面的其他方式。

---

## 🖱️ 交互说明

每个思维导图页面都支持：

- **点击节点文字（或左侧小圆点）** → 折叠 / 展开该节点的子节点；正在选中文字时不会触发，可放心复制；
- 页面**右上角工具栏** → `展开全部` / `只看一级` 一键切换（先看一级骨架，再逐层展开细节）；
- 图片已内联进 HTML，离线也能显示；公式由 KaTeX 渲染，字体走 CDN，联网显示更佳。

---

## 🚀 开启 GitHub Pages（一次性配置）

仓库里已经放好了落地页 `index.html` 和 `.nojekyll`，你只需要在 GitHub 上点几下：

1. 打开仓库 → **Settings**（设置）
2. 左侧栏 → **Pages**
3. **Source** 选 `Deploy from a branch`
4. **Branch** 选 `main`，目录选 `/ (root)`，点 **Save**
5. 等 1–2 分钟，访问 **<https://mingxuanjin.github.io/LC-notes/>**

之后每次 `git push`，Pages 会自动重新发布，链接永久有效。

> 命令行等价操作（需先 `gh auth login`）：
>
> ```bash
> gh api -X POST repos/MingxuanJin/LC-notes/pages \
>   -f source.branch=main -f source.path=/
> ```

---

## 🌐 即时预览（无需任何配置）

### 方式一：htmlpreview 在线预览

把 GitHub 上某个笔记的地址前面加上 `https://htmlpreview.github.io/?` 即可直接渲染，例如：

```
https://htmlpreview.github.io/?https://github.com/MingxuanJin/LC-notes/blob/main/advanced-cl-and-llm/01-wsd.html
```

适合临时分享；长期使用还是推荐 GitHub Pages。

### 方式二：本地打开（无需联网）

```bash
git clone https://github.com/MingxuanJin/LC-notes.git
cd LC-notes
python3 -m http.server 8000
```

然后浏览器访问 `http://localhost:8000/`（落地页），或直接双击任意 `.html` 文件。

> 直接双击打开（`file://`）也能正常看，交互脚本不依赖服务器。

### 方式三：VS Code 实时预览

用 VS Code 打开该文件夹，安装 **Live Preview** 或 **Live Server** 扩展，右键 `.html` → *Show Preview*。改笔记时可以实时刷新。

---

## 🗂️ 仓库结构

```
LC-notes/
├── README.md                      # 本文件
├── index.html                     # GitHub Pages 落地页（可搜索的笔记目录）
├── .nojekyll                      # 让 Pages 原样发布 HTML，跳过 Jekyll
├── .gitignore                     # 忽略 .DS_Store 等
└── advanced-cl-and-llm/           # 笔记正文（自包含思维导图）
    ├── 01-wsd.html
    ├── 02-embeddings.html
    ├── 03-distributional-semantics.html
    ├── 04-glossary.html
    ├── 05-anaphora-coreference.html
    ├── 06-ner.html
    └── 07-llod.html
```

---

## 📝 笔记内容概览

<details>
<summary><b>01 · WSD — Word Sense Disambiguation（词义消歧）</b></summary>

1. Motivation, History, Definition & Tasks
2. Why WSD is Difficult & The 4 Elements of the WSD Workflow
3. Supervised Methods (Classifiers / Word Experts)
4. Minimally and Semisupervised WSD
5. Unsupervised Methods (Word Sense Discrimination)
6. Knowledge-Based WSD
7. Evaluation Frameworks
8. Real-World Applications of WSD

</details>

<details>
<summary><b>02 · Embeddings — 词表示与 LLM 基础</b></summary>

1. From Explicit to Implicit（范式转移）
2. Representing Words
3. Constructing VSMs
4. Evaluation of Word Embeddings
5. Graph Embeddings
6. Sense Embedding
7. Contextualized Embeddings
8. Transformer Architecture
9. Pre-training: Transformers as Language Models
10. Knowledge Injection
11. Prompt Optimization
12. Sentence Embeddings

</details>

<details>
<summary><b>03 · DS — Distributional Semantics（分布语义学）</b></summary>

- Section 1: What is Distributional Semantics?
- Section 2: Distributional Representations
- Section 3: Distributional Semantic Models (DSMs)
- Section 4: Neural Network Models
- Section 5: Evaluation of Distributional Semantic Models

</details>

<details>
<summary><b>04 · Glossary — 术语表</b></summary>

- Computer & Algorithm Basics
- Artificial Intelligence (AI) Taxonomy
- Machine Learning & Paradigms
- Neural Networks & Deep Learning
- Vector Semantics & Embeddings
- LLM Core Architectures & Mechanisms
- Model Training & Capabilities
- LLM Alignment & Safety Engineering
- Historical Traditions & Neuro-Symbolic AI

</details>

<details>
<summary><b>05 · AR & CR — 回指与共指消解</b></summary>

1. Core Terminology (The Foundations)
2. AR vs. CR (The Core Debate)
3. Types of References (The Variations)
4. Constraints for Resolution (The Filters)
5. Datasets (The Gold Standards)
6. Reference Resolution Algorithms & Tools

</details>

<details>
<summary><b>06 · NER — 命名实体识别</b></summary>

1. Origin and Definition of Named Entity (NE)
2. Entity Types
3. Learning Methods for NER
4. NER Features
5. NER Evaluation & Error Types

</details>

<details>
<summary><b>07 · LLOD — Linguistic Linked Open Data</b></summary>

1. Motivation & The FAIR Principles
2. Linked Data (LD) & The Semantic Web
3. Resource Description Framework (RDF) & RDFS
4. Interoperability & LLOD Cloud
5. Advanced Linguistic Models & Metadata
6. OLiA (Ontologies for Linguistic Annotation)
7. Lifecycle of Publishing Linguistic Linked Data
8. SPARQL Keywords & Best Practices

</details>

---

## 📄 说明

- 笔记内容为个人学习整理，思维导图由工具导出为静态 HTML。
- 原始导出中的图片是幕布 CDN 外链（有防盗链，在 GitHub Pages 上会 403 裂图），现已**下载并内联为 base64**，因此每份笔记都是真正的单文件，离线／任意域名下都能显示。
- 折叠 / 展开交互是一段注入的轻量脚本（CSS 与 JS 均在 `injected: interactive collapse` 注释之间），删除这两段即可还原为原始静态导图。

> 若之后重新从幕布导出覆盖了这些文件，交互脚本和图片内联都会丢失，需要重新处理一遍。
