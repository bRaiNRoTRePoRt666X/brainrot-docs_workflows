# 🧠 SSG Options for Brainrot Docs

**Current brainrot level:** 666x

## Quickstart
1. `pip install mkdocs mkdocs-material`
2. `mkdocs serve`
3. Push to `main` → auto-deploys to GitHub Pages.

Brainrot level: MAXIMUM. WEE-OOO.

---

## 🔄 Alternative SSG Options

MkDocs too basic for your brainrot empire? Here are the top 4 GitHub-native drop-ins:

| SSG | Best For | Speed | Setup |
|-----|----------|-------|-------|
| **MkDocs** | Python docs, simplicity | ⚡⚡⚡ | `pip install` |
| **Docusaurus** | React/MDX, versioning, i18n | ⚡⚡⚡⚡ | `npx create-docusaurus` |
| **Hugo** | Raw speed, massive archives | ⚡⚡⚡⚡⚡ | `hugo new site` |
| **Sphinx** | Python API docs, reST | ⚡⚡⚡ | `pip install sphinx` |
| **VitePress** | Vue + Vite speed | ⚡⚡⚡⚡ | `npm init vitepress` |

---

## Option 1: Docusaurus 📘

**React/MDX powerhouse — versioning, search, i18n built-in. 2026 docs king**

### Install
```bash
npx create-docusaurus@latest . classic --typescript
```

### Config (docusaurus.config.ts)
```ts
module.exports = {
  title: 'Brainrot Docs 666X',
  tagline: 'TikTok brainrot reports go brrr',
  url: 'https://bRaiNRoTRePoRt666X.github.io',
  baseUrl: '/brainrot-docs_workflows/',
  onBrokenLinks: 'throw',
  presets: [['classic', { docs: { sidebarPath: require.resolve('./sidebars.js') } }]],
};
```

### Workflow
See: `.github/workflows/docusaurus-deploy.yml`

---

## Option 2: Hugo ⚡

**Blazing fast Go beast — 100k pages in seconds. Perfect for massive brainrot archives**

### Install
```bash
hugo new site . --force
hugo new content/_index.md
```

### Config (config.yaml)
```yaml
baseURL: 'https://bRaiNRoTRePoRt666X.github.io/brainrot-docs_workflows/'
title: Brainrot Docs 666X
theme: hugo-geekdoc
```

### Workflow
See: `.github/workflows/hugo-deploy.yml`

---

## Option 3: Sphinx 🐍

**Python reST beast — auto-API docs, if your brainrot has code**

### Install
```bash
pip install sphinx sphinx-rtd-theme
sphinx-quickstart --quiet
```

### Config (conf.py)
```python
project = 'Brainrot Docs 666X'
extensions = ['sphinx.ext.autodoc']
html_theme = 'sphinx_rtd_theme'
```

### Workflow
See: `.github/workflows/sphinx-deploy.yml`

---

## Option 4: VitePress ⚡

**Vue + Vite speedrun — lightweight + modern**

### Install
```bash
npm init vitepress@latest .
```

### Config (.vitepress/config.ts)
```ts
export default {
  title: 'Brainrot Docs 666X',
  description: 'TikTok brainrot reports',
}
```

### Workflow
See: `.github/workflows/vitepress-deploy.yml`

---

## Migration Guide

### From MkDocs → Docusaurus
```bash
# 1. Backup current config
mv mkdocs.yml mkdocs.yml.bak

# 2. Install Docusaurus
npx create-docusaurus@latest . classic --typescript

# 3. Copy your docs
cp -r docs/* docs-md/

# 4. Update workflow
# Use docusaurus-deploy.yml

# 5. Push
git add .
git commit -m "Migrate to Docusaurus"
git push
```

### From MkDocs → Hugo
```bash
# 1. Install Hugo
# 2. Move content
mkdir content
cp -r docs/* content/

# 3. Use hugo-deploy.yml
```

---

## Benchmarks (2026)

| Metric | MkDocs | Docusaurus | Hugo | Sphinx | VitePress |
|--------|--------|------------|------|--------|-----------|
| Build Speed (1k pages) | 30s | 45s | 5s | 60s | 15s |
| Bundle Size | Medium | Large | Tiny | Large | Small |
| Learning Curve | Low | Medium | Low | High | Low |
| Plugin Ecosystem | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐ |

**Verdict:** Hugo for raw speed, Docusaurus for React brains, Sphinx for Python purity, VitePress for Vue fans.

BWOOP — pick your fighter! WEE-OOO! 🚀
