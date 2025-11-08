---
permalink: /
title: ""              # 仅显示站点名（Xiaolong Li）
excerpt: "Xiaolong Li"
author_profile: true
redirect_from:
  - /about/
  - /about.html
layout: single
---

<style>
:root{
  --text:#1d1d1f;
  --muted:#555559;
  --link:#0066cc;
  --line:#d2d2d7;
  --card:#ffffff;
  --shadow:0 6px 14px rgba(0,0,0,.03);
  --radius:14px;
}

/* 基础排版（更紧凑） */
.page__content{
  font-family:-apple-system,BlinkMacSystemFont,"SF Pro Text","Helvetica Neue",
               Arial,"PingFang SC","Hiragino Sans GB","Microsoft YaHei",sans-serif;
  color:var(--text);
  background:transparent;
  padding:4px;
  font-size:15px;
  line-height:1.6;
}
.page__content h1{font-size:32px;margin:0 0 6px;}
.page__content h2{font-size:20px;font-weight:700;margin:20px 0 10px;}
.page__content h3{font-size:18px;margin:12px 0 6px;}
.page__content a{color:var(--link);text-decoration:none;}
.page__content a:hover{text-decoration:underline;}

/* 顶部简介 */
.hero{margin:0 0 10px;}
.hero h1{font-size:34px;font-weight:700;margin:0 0 6px;}
.hero .sub{font-size:15px;line-height:1.6;color:var(--muted);}
.hero .mono{font-weight:600;color:var(--text);}

/* 白卡片 */
.card{
  background:var(--card);
  border:1px solid var(--line);
  border-radius:var(--radius);
  box-shadow:var(--shadow);
  padding:14px 16px;
}

/* Education：左文/中日期/右logo */
.edu-row{
  display:grid;
  grid-template-columns:1fr auto auto;
  column-gap:12px;
  align-items:center;
  padding:10px 0;
}
.edu-title{font-weight:600;font-size:16px;margin:0 0 2px;}
.edu-sub{font-style:italic;color:var(--muted);font-size:14px;margin:0;}
.edu-date{text-align:right;font-weight:600;color:#3d3d40;font-size:14px;white-space:nowrap;}
.edu-right{text-align:right;}
.logo{height:40px;object-fit:contain;display:block;margin-left:auto;}
.logo.ubc{transform:scale(1.1);transform-origin:right center;}

/* Publications */
.pub{display:grid;gap:6px;font-size:15px;}
.pub + .pub{border-top:1px solid var(--line);padding-top:12px;margin-top:12px;}
.pub-title{font-weight:700;font-size:15px;}
.pub-authors{color:var(--muted);font-size:14px;}
.pub-venue{color:var(--link);font-weight:600;font-size:14px;}

/* 银灰胶囊按钮 */
.chips{display:flex;gap:8px;margin-top:6px;flex-wrap:wrap;}
.chip{
  display:inline-block;padding:6px 12px;border-radius:999px;
  background:#f5f5f7;border:1px solid #c7c7cc;color:#1d1d1f;
  font-weight:600;font-size:13px;text-decoration:none;
  box-shadow:0 1px 0 rgba(255,255,255,.8) inset;
  transition:transform .12s ease,background .12s ease;
}
.chip:hover{transform:translateY(-1px);background:#f8f8fa;}

.item + .item{border-top:1px solid var(--line);padding-top:10px;margin-top:10px;}

/* —— 修复顶部空白 & 正文右移 —— */
.initial-content{padding-top:8px !important;margin-top:0 !important;}
.page__hero,.page__hero--overlay{display:none !important;height:0 !important;margin:0 !important;padding:0 !important;}
.layout--single .page__inner-wrap{padding-top:0 !important;margin-top:0 !important;}
.page__content{margin-top:0 !important;}

/* 强制隐藏空的 header 和 page__title */
.page__inner-wrap > header{display:none !important;height:0 !important;margin:0 !important;padding:0 !important;}
.page__title{display:none !important;height:0 !important;margin:0 !important;padding:0 !important;line-height:0 !important;}

/* 彻底消除顶部留白 */
#main{
  margin-top:0 !important;
  padding-top:0.5em !important;
}
article.page{margin-top:0 !important;padding-top:0 !important;}
.sidebar{margin-top:0 !important;padding-top:0 !important;}

/* 主内容容器（与 author card 对齐） */
.content-container{
  background:transparent;
  border:none;
  border-radius:16px;
  box-shadow:none;
  padding:32px;
  margin:0;
  width:100%;  /* 填满父容器宽度 */
  max-width:1200px;  /* 限制最大宽度 */
  box-sizing:border-box;  /* 确保padding计算在width内 */
}

/* 确保 page__content 不会有多余的 padding，并填满宽度 */
.page__content{
  padding:0 !important;
  width:100% !important;
  max-width:none !important;
}

/* 确保 article.page 也填满可用宽度 */
article.page{
  width:100% !important;
}

/* 强制让sidebar和page顶部对齐 */
@media (min-width:64em){
  #main{
    display:flex !important;
    align-items:flex-start !important;
    gap:0 !important;
    max-width: 1800px !important;  /* 更大的最大宽度 */
    width: 100% !important;
    padding-left: 2em !important;
    padding-right: 2em !important;
  }

  .sidebar{
    flex:0 0 260px !important;  /* 减小sidebar到260px */
    margin-top:0 !important;
    padding-top:0 !important;
    margin-right:30px !important;  /* 增加间距 */
  }

  article.page{
    flex:1 1 0 !important;  /* 关键：flex-basis设为0让它填满剩余空间 */
    margin-top:0 !important;
    padding-top:0 !important;
    margin-left:0 !important;
    max-width: none !important;
    min-width: 0 !important;  /* 允许收缩 */
  }

  /* 强制移除page__inner-wrap的宽度限制 */
  .page__inner-wrap{
    max-width: none !important;
    width: 100% !important;
  }
}

/* 移动端堆叠 */
@media (max-width:720px){
  .edu-row{grid-template-columns:1fr;row-gap:6px;}
}
</style>

<div class="content-container">

<div class="hero">
  <h1>About Me</h1>
  <p class="sub">
    I am a first-year Ph.D. student in Computer Science at <span class="mono">The University of Hong Kong (HKU)</span>,
    advised by <a href="https://www.reynold.hku.hk/" target="_blank">Professor Reynold C.K. Cheng</a>.
    My research focuses on <span class="mono">data-centric code generation</span>: Text-to-SQL, code agents, and automated data science workflows.
  </p>
  <p class="sub" style="margin-top:8px;">
    <strong>Contact:</strong> xia01ong[AT]connect.hku.hk
  </p>
</div>

<h2>Education</h2>
<div class="card">
  <div class="edu-row">
    <div class="edu-left">
      <p class="edu-title">The University of Hong Kong</p>
      <p class="edu-sub">Ph.D in Department of Computer Science</p>
    </div>
    <div class="edu-date">2025-Sep. – Now</div>
    <div class="edu-right"><img class="logo" src="/edu_logo/hku.jpg" alt="HKU"></div>
  </div>

  <div class="edu-row">
    <div class="edu-left">
      <p class="edu-title">The University of Hong Kong</p>
      <p class="edu-sub">Master of Science in Computer Science (General Track)</p>
    </div>
    <div class="edu-date">2023-Sep. – 2024-Nov.</div>
    <div class="edu-right"><img class="logo" src="/edu_logo/hku.jpg" alt="HKU"></div>
  </div>

  <div class="edu-row">
    <div class="edu-left">
      <p class="edu-title">The University of British Columbia</p>
      <p class="edu-sub">Bachelor of Science in Computer Science</p>
    </div>
    <div class="edu-date">2019-Sep. – 2023-May</div>
    <div class="edu-right"><img class="logo ubc" src="/edu_logo/ubc.jpg" alt="UBC"></div>
  </div>
</div>

<h2>Publications</h2>
<div class="card">
  <ol style="margin:0;padding-left:20px;">
    <li class="pub">
      <div class="pub-title">BIRD-INTERACT: Re-imagining Text-to-SQL Evaluation via Lens of Dynamic Interactions</div>
      <div class="pub-authors">
        Nan Huo, Xiaohan Xu, Jinyang Li, Per Jacobsson, Shipei Lin, Bowen Qin, Binyuan Hui,
        <strong><em><u>Xiaolong Li</u></em></strong>, Ge Qu, Shuzheng Si, Linheng Han, Edward Alexander, Xintong Zhu,
        Rui Qin, Ruihan Yu, Yiyao Jin, Feige Zhou, Weihao Zhong, Yun Chen, Hongyu Liu, Chenhao Ma, Fatma Ozcan,
        Yannis Papakonstantinou, Reynold Cheng
      </div>
      <div class="pub-venue"><a href="https://arxiv.org/abs/2510.05318" target="_blank">Arxiv 2025</a></div>
      <div class="chips">
        <a class="chip" href="https://arxiv.org/abs/2510.05318" target="_blank">Paper</a>
        <a class="chip" href="https://bird-interact.github.io/" target="_blank">Code</a>
      </div>
    </li>

    <li class="pub">
      <div class="pub-title">SWE-SQL: Illuminating LLM Pathways to Solve User SQL Issues in Real-World Applications</div>
      <div class="pub-authors">
        Jinyang Li*, <strong><em><u>Xiaolong Li</u></em></strong>*, Ge Qu*, Per Jacobsson, Bowen Qin, Binyuan Hui, Shuzheng Si,
        Nan Huo, Xiaohan Xu, Yue Zhang, Ziwei Tang, Yuanshuai Li, Florensia Widjaja, Xintong Zhu, Feige Zhou, Yongfeng Huang,
        Yannis Papakonstantinou, Fatma Ozcan, Chenhao Ma, Reynold Cheng
      </div>
      <div class="pub-venue">NeurIPS Main 2025</div>
      <div class="chips">
        <a class="chip" href="https://arxiv.org/abs/2506.18951" target="_blank">Paper</a>
        <a class="chip" href="https://bird-critic.github.io/" target="_blank">Code</a>
      </div>
    </li>

    <li class="pub">
      <div class="pub-title">SHARE: An SLM-based Hierarchical Action CorREction Assistant for Text-to-SQL</div>
      <div class="pub-authors">
        Ge Qu, Jinyang Li, Bowen Qin, <strong><em><u>Xiaolong Li</u></em></strong>, Nan Huo, Chenhao Ma, Reynold Cheng
      </div>
      <div class="pub-venue">ACL Main 2025</div>
      <div class="chips">
        <a class="chip" href="https://arxiv.org/abs/2506.00391" target="_blank">Paper</a>
        <a class="chip" href="https://github.com/quge2023/SHARE" target="_blank">Code</a>
      </div>
    </li>

    <li class="pub">
      <div class="pub-title">Micro-Act: Mitigate Knowledge Conflict in Question Answering via Actionable Self-Reasoning</div>
      <div class="pub-authors">
        Nan Huo, Jinyang Li, Bowen Qin, Ge Qu, <strong><em><u>Xiaolong Li</u></em></strong>, Xiaodong Li, Chenhao Ma, Reynold Cheng
      </div>
      <div class="pub-venue">ACL Main 2025</div>
      <div class="chips">
        <a class="chip" href="https://arxiv.org/abs/2506.05278" target="_blank">Paper</a>
        <a class="chip" href="https://github.com/Noah-Flame/Micro-Act" target="_blank">Code</a>
      </div>
    </li>
  </ol>
</div>

<h2>Research Project</h2>
<div class="card">
  <div class="item">
    <p><a href="https://github.com/bird-bench/mini_dev" target="_blank"><strong>BIRD-SQL Mini-Dev</strong></a>: A Multilingual, Lightweight Version of the BIRD Development Set</p>
    <p style="font-size:14px;color:var(--muted);margin-bottom:8px;">May 2024 — Aug 2024</p>
    <ul>
      <li><strong>Update 2025-07-22</strong>: Released V2 with 780 instances (500 SELECT-only + 270 CRUD across 18 DBs). Added JSON ops and multi-dialect support (PostgreSQL, SQLite). See <a href="https://livesqlbench.ai/" target="_blank">LiveSQLBench</a>.</li>
      <li>A lite development set for fast, cost-effective Text-to-SQL iteration. 500 high-quality pairs across 11 DBs in MySQL & PostgreSQL. Introduces R-VES (efficiency) and Soft-F1 (accuracy).</li>
    </ul>
    <div class="chips">
      <a class="chip" href="https://github.com/bird-bench/mini_dev" target="_blank">GitHub</a>
      <a class="chip" href="https://huggingface.co/datasets/birdsql/bird_mini_dev" target="_blank">HuggingFace</a>
    </div>
  </div>
</div>

<h2>Awards & Honors</h2>
<div class="card">
  <ul>
    <li><strong>Postgraduate Scholarship (PGS)</strong> — The University of Hong Kong, 2025</li>
    <li><strong>Dean’s Honour List</strong> — University of British Columbia, 2021</li>
    <li><strong>Graduate with Distinction</strong> — UBC (B.Sc.) & HKU (M.Sc.)</li>
  </ul>
</div>

<p style="color:var(--muted);font-style:italic">Last updated: Nov 2025</p>

</div> <!-- /content-container -->
