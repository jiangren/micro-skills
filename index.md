---
layout: home
title: 我的微技能日志
---

> 基于罗伯特·特威格尔《微精通》——每周设计一个 **3–5 小时可完成**、有明确"最小可演示成果"的微技能方案。

## 历史方案

<ul>
{% assign plans = site.pages | where_exp: "p", "p.path contains '微技能方案-'" | sort: "path" | reverse %}
{% for plan in plans %}
  <li>
    <a href="{{ plan.url | relative_url }}">{{ plan.title | default: plan.path | replace: '.md', '' }}</a>
  </li>
{% endfor %}
</ul>

---

## 关于这个站点

- 每周一篇方案，存放为独立的 `.md` 文件
- 通过 GitHub Actions（或本地脚本）自动发布到 GitHub Pages
- 主题：Jekyll [Minima](https://github.com/jekyll/minima)

[查看源仓库 →](https://github.com/jiangren/micro-skills)
