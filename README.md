# 课程考试复习指南 Skill

这是一个面向中文母语者的 Codex skill，用于帮助大家整理老师的课件、资料与复习题，并生成可直接备考的复习包。它会优先围绕“考试怎么答题”来分析材料，而不是只做普通摘要。

适合处理：

- 课件、讲义、笔记、教材
- PDF、Word、Excel、PPT
- 复习题、作业、往年试卷、答案、评分标准
- 图片、截图、扫描件
- 包含课程资料的压缩包

## 适合做什么

- 逐题整理题目来源、知识点、题型识别、标准公式/定义/规则、解题方法、步骤、答案和常见错误
- 为期末、期中、测验和课程考试生成复习文档
- 从压缩包里分析课程资料，并整理成结构化学习材料
- 生成公式/定义/规则/框架速查表
- 支持理工、商科、法律、医学、人文、语言等学科

## 典型触发方式

可以直接对 Codex 说：

- `使用 $course-exam-study-guide 分析这些课程资料`
- `彻底分析压缩包`
- `把这份课件和往年题整理成考试复习指南`
- `根据这些题目和答案做逐题解析`
- `帮我把这些课程文件做成期末复习资料`

## 输出内容

通常包括：

- 公式/定义/规则/框架速查表
- 每道题的知识点、题型识别和标准解法
- 考试可直接执行的步骤
- 答案或模型结论
- 常见错误和材料来源

## 安装

### Windows PowerShell

把本仓库克隆到 Codex skills 目录：

```powershell
git clone https://github.com/xufu111/course-exam-study-guide.git "$env:USERPROFILE\.codex\skills\course-exam-study-guide"
```

安装后重启 Codex。

### macOS / Linux

```bash
git clone https://github.com/xufu111/course-exam-study-guide.git ~/.codex/skills/course-exam-study-guide
```

安装后重启 Codex。

## 使用建议

- 如果你有一个课程资料压缩包，可以直接说：`彻底分析压缩包`。
- 如果资料里有答案或评分标准，一起提供，结果会更接近老师预期。
- 如果 PDF 是扫描件，分析结果可能受 OCR 质量影响；重要题目建议人工抽查。
- 如果公式很多，建议要求输出 Markdown、LaTeX 或 PDF，方便保留数学格式。

## 文件结构

```text
course-exam-study-guide/
├── SKILL.md
├── README.md
└── agents/
    └── openai.yaml
```

## 说明

`SKILL.md` 顶部的 `name` 和 `description` 是 Codex 用来识别和触发 skill 的元数据；它们在某些 Markdown 预览器里会显示出来，这是正常的。
