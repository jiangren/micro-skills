# micro-skills

每周一个《微精通》方法论的微技能学习方案。3–5 小时可完成，有明确的"最小可演示成果"。

**👉 在线阅读**: https://jiangren.github.io/micro-skills/

## 工作流程

1. Cowork 每周自动生成一份 `微技能方案-YYYY-MM-DD-技能名.md`
2. 推到 `main` 分支
3. GitHub Pages（Jekyll + minima 主题）自动构建并发布

## 本地预览

```bash
gem install bundler jekyll
bundle init
bundle add jekyll minima
bundle exec jekyll serve
```

## 目录结构

```
.
├── _config.yml                       # Jekyll 配置
├── index.md                          # 首页（按时间倒序列出所有方案）
├── README.md                         # 你正在读这个
└── 微技能方案-*.md                   # 每周一篇方案
```
