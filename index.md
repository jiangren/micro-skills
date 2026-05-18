---
title: 首页
layout: default
nav_order: 1
---

# 我的微技能日志
{: .fs-9 }

每周一个 **3-5 小时可完成**、有明确"最小可演示成果"的微技能学习方案。基于罗伯特·特威格尔《微精通》方法论。
{: .fs-5 .fw-300 }

[最新方案](#最新方案){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[查看 GitHub 仓库](https://github.com/jiangren/micro-skills){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## 这是什么

微精通(Micromastery)主张:不要追求宏大目标,而是把一个**完整、可演示、有正反馈**的小技能片段在几小时内学到能拿出手。每个微技能由 6 个要素构成——入门技巧、协同障碍、辅助支持、回报奖励、可复验性、可实验性。

本站记录我每周尝试的一个微技能。

## 最新方案

<ul class="docs-list">
{% assign plans = site.pages | where: "parent", "历史方案" | sort: "title" | reverse %}
{% for plan in plans limit:3 %}
  <li><a href="{{ plan.url | relative_url }}"><strong>{{ plan.title }}</strong></a></li>
{% endfor %}
</ul>

完整列表见左侧"**历史方案**"分组。

## 工作流

1. Cowork 每周自动生成一份新的微技能方案 `.md` 文件
2. 推到 `main` 分支
3. GitHub Pages 自动构建并发布
