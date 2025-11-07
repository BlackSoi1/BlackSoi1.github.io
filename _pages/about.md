---
permalink: /
title: ""              # 置空以只显示 site.title（Xiaolong Li）
excerpt: "Xiaolong Li"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
:root{
  --text:#1d1d1f;
  --muted:#555559;
  --link:#0066cc;
  --line:#d2d2d7;
  --card:#ffffff;
  --page-bg:#fff;              /* 纯白 */
  --shadow:0 10px 22px rgba(0,0,0,.04);
  --radius:16px;
}

.page__content{
  font-family:-apple-system,BlinkMacSystemFont,"SF Pro Text","Helvetica Neue",
               Arial,"PingFang SC","Hiragino Sans GB","Microsoft YaHei",sans-serif;
  color:var(--text);
  background: transparent;     /* 不再上底色 */
  border-radius: var(--radius);
  padding:4px;
}

.page__content h1,.page__content h2,.page__content h3{
  letter-spacing:-.02em;
  color:var(--text);
}

/* 之前的 hr 块感知为“灰色区域”，这里直接禁用 */
.hr{height:0.5px;background:#eee;border:0;margin:20px 0}


/* 顶部介绍 */
.hero{margin-top:8px;margin-bottom:10px}
.hero h1{font-size:clamp(30px,4.2vw,42px);font-weight:700;margin:0 0 6px}
.hero .sub{font-size:clamp(16px,2vw,18px);line-height:1.65;color:var(--muted)}
.hero .mono{font-weight:600;color:var(--text)}

/* Email 胶囊 */
.mail{
  display:inline-flex;align-items:center;gap:8px;
  padding:10px 16px;border-radius:999px;
  background:#f5f5f7;border:1px solid var(--line);
  color:var(--text);font-weight:700;font-size:14px;
  box-shadow:0 1px 0 rgba(255,255,255,.8) inset,var(--shadow);
  transition:transform .12s ease,background .12s ease;
  text-decoration:none;
}
.mail:hover{transform:translateY(-1px);background:#f8f8fa}

/* 区块标题：去掉底部灰线 */
h2{
  font-size:22px;font-weight:800;margin:4px 0 10px;
  padding-bottom:0; border-bottom:0;
}

/* 卡片 */
.card{
  background:var(--card);
  border:1px solid var(--line);
  border-radius:var(--radius);
  box-shadow:var(--shadow);
  padding:18px;
}

/* ===== Education（Grid：左文本/中年份/右logo） ===== */
.edu-row{
  display:grid;
  grid-template-columns: 1fr minmax(0, max-content) 96px;
  column-gap:6px;
  align-items:center;
  padding:14px 0;
}
.edu-left{min-width:0}
.edu-title{font-weight:700;font-size:18px;margin:0 0 4px}
.edu-sub{font-style:italic;color:var(--muted);margin:0}
.edu-date{
  text-align:left;
  font-weight:700;color:#3d3d40;white-space:nowrap;
}
.edu-right{display:flex;justify-content:flex-end;align-items:center}
.logo{height:48px;object-fit:contain;display:block}
.logo.ubc{transform:scale(1.12);transform-origin:right center}

/* Publications */
.pub{display:grid;gap:8px}
.pub + .pub{border-top:1px solid var(--line);padding-top:16px;margin-top:16px}
.pub-title{font-weight:800}
.pub-authors{color:var(--muted)}
.pub-venue{color:var(--link);font-weight:600}

/* 银灰胶囊按钮 */
.chips{display:flex;gap:10px;margin-top:8px;flex-wrap:wrap}
.chip{
  display:inline-block;padding:8px 14px;border-radius:999px;
  background:#f5f5f7;border:1px solid #c7c7cc;color:#1d1d1f;
  font-weight:700;font-size:13px;text-decoration:none;
  box-shadow:0 1px 0 rgba(255,255,255,.8) inset;
  transition:transform .12s ease,background .12s ease;
}
.chip:hover{transform:translateY(-1px);background:#f8f8fa}

/* 项目 */
.item + .item{border-top:1px solid var(--line);padding-top:14px;margin-top:14px}
.page__content a{color:var(--link);text-decoration:none}
.page__content a:hover{text-decoration:underline}

/* 移动端 */
@media (max-width: 720px){
  .edu-row{ grid-template-columns: 1fr; row-gap:6px; }
  .edu-right{justify-content:flex-start}
}
</style>

<div class="hero">
  <h1>Xiaolong Li</h1>
  <p class="sub">
    I am a first-year Ph.D. student in Computer Science at <span class="mono">The University of Hong Kong (HKU)</span>,
    advised by <a href="https://www.reynold.hku.hk/" target="_blank">Professor Reynold C.K. Cheng</a>.
    My research focuses on <span class="mono">data-centric code generation</span>: Text-to-SQL, code agents, and automated data science workflows.
  </p>
  <p><a class="mail" href="mailto:xia01ong@connect.hku.hk">✉️ xia01ong[AT]connect.hku.hk</a></p>
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
