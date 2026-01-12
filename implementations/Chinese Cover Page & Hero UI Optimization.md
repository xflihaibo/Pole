---
title: Chinese Cover Page & Hero UI Optimization
type: note
permalink: implementations/chinese-cover-page-hero-ui-optimization
---

Optimized the landing (cover) page for a premium, Chinese-first experience.
Key Changes:
- **Language**: Full Chinese localization for titles, slogans, and button text.
- **Typography**: Optimized font stack for Chinese rendering (PingFang SC, Microsoft YaHei).
- **Hero Section**:
    - Replaced static background with a **Dynamic Moving Gradient** (animated via CSS keyframes).
    - Added high-contrast typography with a subtle text gradient.
    - Designed custom **Capsule Buttons** with glassmorphism and shadow effects.
- **Docsify Config**:
    - Set `onlyCover: true` to make the landing page the focal point.
    - Updated UI strings (site name, search placeholder) to Chinese.
