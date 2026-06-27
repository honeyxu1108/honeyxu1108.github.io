---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<style>
    #homepage,
    #about-me,
    #news,
    #publications,
    #honors-and-awards,
    #educations {
        scroll-margin-top: 80px;
    }
  
      /* ===== News Scroll Box ===== */
    .news-box {
      max-height: 220px;
      overflow-y: auto;
      padding: 10px 14px;
      background: #f7f7f7;
      border-radius: 10px;
      margin-bottom: 20px;
    }
    
    .news-list {
      list-style: none;
      padding: 0;
      margin: 0;
    }
    
    .news-list li {
      margin-bottom: 10px;
      line-height: 1.5;
    }
    
    .news-date {
      display: inline-block;
      min-width: 70px;
      font-weight: 400;        /* 不加粗 */
      color: #ca6f6f;          /* 浅粉色 */
    }
  
    .experience-card {
        display: flex;
        align-items: center;
        background: #f9f9f9;
        border-radius: 12px;
        padding: 16px;
        margin-bottom: 0px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.05);
        transition: transform 0.3s, box-shadow 0.3s;
    }
    .experience-card:hover {
       
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }
    .experience-logo {
        width: 60px;
        height: 60px;
        margin-right: 20px;
        border-radius: 8px;
        object-fit: contain;
    }
    .experience-info {
        font-family: "Segoe UI", sans-serif;
    }
    .experience-info strong {
        font-size: 1.1em;
    }
    .experience-info a {
        text-decoration: none;
        color: #ca6f6f;
    }
    .experience-container {
        display: flex;
        flex-direction: column; /* 让子元素垂直排列，一行一个 */
        gap: 20px; /* 保持每个卡片之间的间距 */
    }
    .experience-card {
        box-sizing: border-box;
    }
    .publication-card {
        display: flex;
        align-items: center;
        padding: 3px;
        border: 1.5px solid #ddd;
        border-radius: 8px;
        background: #fff;
        box-sizing: border-box;
        margin-bottom: 20px; 
        transition: transform 0.3s ease, box-shadow 0.3s ease;

        color: #5f6368; /* 正文整体更浅 */
    }
    .publication-card > div > strong,
    .publication-card > div > div > strong {
        color: #202124;
    }
    .publication-card i {
        color: #6b7280;
    }

    .pub-badge {
        display: inline-flex;
        align-items: center;
        gap: 0.35em;
        margin-left: 8px;
        padding: 2px 8px;
        border-radius: 999px;
        font-size: 11px;
        font-weight: 650;
        line-height: 1.4;
        letter-spacing: 0.01em;
        vertical-align: middle;
        white-space: nowrap;
        border: 1px solid transparent;
        background: rgba(107, 114, 128, 0.08);
        color: #6b7280;
    }

    .pub-badge::before {
        content: "";
        width: 0.45em;
        height: 0.45em;
        border-radius: 999px;
        background: currentColor;
        opacity: 0.75;
    }

    .pub-badge--oral {
        margin-left: 4px;
        vertical-align: 2px;
        color: #4c6a94;
        background: rgba(131, 161, 199, 0.14);
        border-color: rgba(131, 161, 199, 0.35);
    }
    .publication-card:hover {
       
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }

    .publication-card.featured {
        border-color: #f5bba7;       /* 更浅的哈密瓜色边框 */
        background: #fef5f1;         /* 非常浅的哈密瓜色背景 */
        box-shadow: 0 4px 8px rgba(242, 166, 120, 0.2); /* 更柔和的初始阴影 */
        z-index: 10;
    }

    .publication-card.featured:hover {
        box-shadow: 0 8px 16px rgba(242, 166, 120, 0.4); 
    }
    
    /*.publication-card.non-featured {*/
        /*display: flex;  默认隐藏非精选出版物 */
    /*}*/
    
    .pub-button-container {
        display: flex;
        gap: 10px;
        margin: 20px 0;
        flex-wrap: wrap;
    }
    
    .pub-button {
        background-color: #f0f0f0;
        border: 1px solid #ccc;
        border-radius: 20px;
        padding: 8px 16px;
        cursor: pointer;
        transition: all 0.3s ease;
    }
    
    .pub-button:hover {
        background-color: #e0e0e0;
    }
    
    .pub-button.active {
        background-color: #ca6f6f;
        color: white;
        border-color: #ca6f6f;
    }

      .publication-view[hidden] {
        display: none !important;
    }

      #full-publications {
        max-height: 380px;
        overflow-y: auto;
        padding-right: 8px;
        margin-bottom: 24px;
        scroll-behavior: smooth;
        scrollbar-width: thin;
        scrollbar-color: rgba(185, 95, 61, 0.45) rgba(254, 245, 241, 0.7);
    }

    #full-publications::-webkit-scrollbar {
        width: 8px;
    }

    #full-publications::-webkit-scrollbar-track {
        background: rgba(254, 245, 241, 0.7);
        border-radius: 999px;
    }

    #full-publications::-webkit-scrollbar-thumb {
        background: rgba(185, 95, 61, 0.45);
        border-radius: 999px;
    }

    #full-publications::-webkit-scrollbar-thumb:hover {
        background: rgba(185, 95, 61, 0.65);
    }
  
    .full-publication-list {
        margin: 0;
        padding-left: 1.25rem;
        color: #5f6368;
        font-size: 15px;
        line-height: 1.55;
    }

    .full-publication-list li {
        margin-bottom: 14px;
    }

    .pub-list-badge {
        display: inline-block;
        margin-right: 6px;
        padding: 2px 8px;
        border-radius: 999px;
        border: 1px solid rgba(245, 187, 167, 0.75);
        background: #fef5f1;
        color: #b95f3d;
        font-size: 11px;
        font-weight: 650;
        line-height: 1.35;
        vertical-align: 1px;
        white-space: nowrap;
    }

    .full-publication-list .pub-list-title {
        color: #202124;
        font-size: 15px;
        font-weight: 700;
        line-height: 1.45;
        text-decoration: none !important;
    }

      .pub-list-authors {
        color: #6b7280;
        font-size: 13px;
        font-style: italic;
    }

    .pub-list-authors > strong {
        color: #202124;
    }

      .pub-list-authors a strong {
        color: inherit;
    }

    .pub-list-note {
        color: #c7774c;
        font-style: italic;
        font-weight: 650;
    }

    .pub-list-links {
        white-space: nowrap;
    }

    .pub-list-links a {
        margin-left: 4px;
        color: #c7774c !important;
        font-weight: 600;
    }

      .pub-list-links a:hover {
        color: #b65f36 !important;
    }

    /* Projects cards: keep styles independent from publications */
    .project-card {
        display: flex;
        align-items: center;
        padding: 3px;
        border: 1.5px solid #ddd;
        border-radius: 8px;
        background: #fff;
        box-sizing: border-box;
        margin-bottom: 20px;
        transition: transform 0.3s ease, box-shadow 0.3s ease;

        color: #5f6368;
    }

    .project-card > div > strong,
    .project-card > div > div > strong {
        color: #202124;
    }

    .project-card i {
        color: #6b7280;
    }

    .project-card:hover {
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }

      @media (max-width: 720px) {
        .publication-card,
        .project-card {
            align-items: stretch;
            padding: 8px;
        }

        .publication-card > div,
        .project-card > div {
            flex-direction: column;
            align-items: stretch !important;
            width: 100%;
        }

        .publication-card .pub-media-rotator,
        .project-card .pub-media-rotator {
            width: 100% !important;
            height: auto !important;
            aspect-ratio: 16 / 9;
            margin-right: 0 !important;
            margin-bottom: 12px;
        }

        .publication-card .pub-media-rotator > img,
        .project-card .pub-media-rotator > img {
            width: 100% !important;
            height: 100% !important;
            object-fit: contain;
        }

        .publication-card strong,
        .project-card strong {
            line-height: 1.35;
        }

        .full-publication-list {
            padding-left: 1rem;
        }

        .pub-list-badge {
            margin-bottom: 4px;
        }
    }

  
</style>
<html> 
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Fredericka+the+Great&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Homemade+Apple&display=swap');
        body {
            background-color: #FFFFFF;
            font-family: 'Source Sans 3', 'Noto Sans SC', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            font-size: 15px;
        }
        .main-heading {
            font-family: 'Permanent Marker', cursive;
            text-align: center;
            color: #6CB4E8;
        }
        div.markdown-body a,a {
            text-decoration: none !important;
            color: #ca6f6f;
            transition: all 0.3s ease; /* 平滑过渡效果 */
        }
        div.markdown-body a:hover, a:hover {
            color: #c71585;            /* 悬浮时变深一点的颜色 */
            text-decoration: underline; /* 加上悬浮时的下划线 */
        }
    </style>
</head>
<body>
<h1 id="homepage" class="main-heading">Welcome to my Homepage!</h1>
</body>
</html>

About Me
---------------

Hi! I am a second-year master's student in the <a href="http://www.cs.sjtu.edu.cn"><em>School of Computer Science</em></a> at <a href="https://www.sjtu.edu.cn/"><em>Shanghai Jiao Tong University</em></a>.

Starting from 2024, I am supervised by Prof. <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN"><em>Xiaokang Yang</em></a> and Associate Professor <a href="https://daodaofr.github.io/"><em>Yichao Yan</em></a> at the Institute of Artificial Intelligence. Prior to that, I received my bachelor's degree from <a href="https://www.shu.edu.cn/"><em>Shanghai University</em></a>.

My research interests include **Motion Generation**, **Personal Portrait Animation** and **Computer Vision**. I am also interested in **History** in my spare time.

Feel free to reach out if you are interested in collaboration or potential opportunities.

News
---------------
<div class="news-box">
  <ul class="news-list">
    <li><span class="news-date"><em>2026.03</em></span> 🎉🎉 One paper: SingingBot is accepted by ICME 2026!</li>
    <li><span class="news-date"><em>2025.06</em></span> 🎉🎉 One paper is accepted by ICCV 2025!</li>
  </ul>
</div>

Publications
--------------
<button class="pub-button active" onclick="filterPublications(event, 'all')">Core Publications</button>
<button class="pub-button" onclick="filterPublications(event, 'list')">Full Publications List</button>

(* equal contribution · &dagger; corresponding author · &Dagger; project leader)

<div id="core-publications" class="publication-view" data-publication-view="core">
<div class="publication-card" data-category="all">
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;">
      <img src="images/intervla.jpg" alt="InterVLA" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;">
    </div>
    <div>
      <strong><a href="https://arxiv.org/abs/2508.04681" target="_blank">Perceiving and Acting in First-Person: A Dataset and Benchmark for Egocentric Human-Object-Human Interactions</a></strong><br>
      <i style="font-size: 13px;">
        <a href="https://liangxuy.github.io/" target="_blank">Liang Xu</a>,
        Chengqun Yang,
        Zili Lin,
        <a href="https://honeyxu1108.github.io" target="_blank"><strong>Fei Xu</strong></a>,
        Yifan Liu,
        Congsheng Xu,
        Yiyi Zhang,
        Jie Qin,
        Xingdong Sheng,
        Yunhui Liu,
        Xin Jin,
        <a href="https://daodaofr.github.io/" target="_blank">Yichao Yan</a>,
        Wenjun Zeng,
        <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN" target="_blank">Xiaokang Yang</a>
      </i><br>
      We embed the manual-assisted task into a vision-language-action framework and build InterVLA, the first large-scale human-object-human interaction dataset with 11.4 hours and 1.2M frames of multimodal data, along with benchmarks on egocentric human motion estimation, interaction synthesis, and interaction prediction.
      <br>
      <b><i style="color:#83a1c7;">ICCV 2025 &nbsp;
      </i></b>
      <a href="https://arxiv.org/abs/2508.04681"><em>[arXiv]</em></a>
    </div>
  </div>
</div>

<div class="publication-card" data-category="all">
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;">
      <img src="images/SingingBot.png" alt="SingingBot" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;">
    </div>
    <div>
      <strong><a href="https://arxiv.org/abs/2601.02125" target="_blank">SingingBot: An Avatar-Driven System for Robotic Face Singing Performance</a></strong><br>
      <i style="font-size: 13px;">
        Zhuoxiong Xu,
        Xuanchen Li,
        Yuhao Cheng,
        <a href="https://honeyxu1108.github.io" target="_blank"><strong>Fei Xu</strong></a>,
        <a href="https://daodaofr.github.io/" target="_blank">Yichao Yan</a>,
        <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN" target="_blank">Xiaokang Yang</a>
      </i><br>
      We propose an avatar-driven framework for appealing robotic singing that synthesizes vivid singing avatars for expression guidance and transfers facial features to the robot via semantic-oriented mapping, achieving rich emotional expressions while maintaining lip-audio synchronization.
      <br>
      <b><i style="color:#83a1c7;">ICME 2026 &nbsp;
      </i></b>
      <a href="https://arxiv.org/abs/2601.02125"><em>[arXiv]</em></a>
    </div>
  </div>
</div>

</div>
<div id="full-publications" class="publication-view" data-publication-view="list" hidden>
  <ul class="full-publication-list">
    <li>
      <span class="pub-list-badge">ICCV 2025</span>
      <a class="pub-list-title" href="https://arxiv.org/abs/2508.04681" target="_blank">Perceiving and Acting in First-Person: A Dataset and Benchmark for Egocentric Human-Object-Human Interactions</a><br>
      <span class="pub-list-authors">
        <a href="https://liangxuy.github.io/" target="_blank">Liang Xu</a>, Chengqun Yang, Zili Lin,
        <a href="https://honeyxu1108.github.io" target="_blank"><strong>Fei Xu</strong></a>,
        Yifan Liu, Congsheng Xu, Yiyi Zhang, Jie Qin, Xingdong Sheng, Yunhui Liu, Xin Jin,
        <a href="https://daodaofr.github.io/" target="_blank">Yichao Yan</a>, Wenjun Zeng,
        <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN" target="_blank">Xiaokang Yang</a>.
      </span>
      <span class="pub-list-links"><a href="https://arxiv.org/abs/2508.04681">[arXiv]</a></span>
    </li>
    <li>
      <span class="pub-list-badge">ICME 2026</span>
      <a class="pub-list-title" href="https://arxiv.org/abs/2601.02125" target="_blank">SingingBot: An Avatar-Driven System for Robotic Face Singing Performance</a><br>
      <span class="pub-list-authors">
        Zhuoxiong Xu, Xuanchen Li, Yuhao Cheng,
        <a href="https://honeyxu1108.github.io" target="_blank"><strong>Fei Xu</strong></a>,
        <a href="https://daodaofr.github.io/" target="_blank">Yichao Yan</a>,
        <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN" target="_blank">Xiaokang Yang</a>.
      </span>
      <span class="pub-list-links"><a href="https://arxiv.org/abs/2601.02125">[arXiv]</a></span>
    </li>
  </ul>
</div>

<script src="assets/js/show_publications.js"></script>
<script src="assets/js/pub_media_rotator.js"></script>

Honors and Awards
--------------
- *Coming soon.*

Educations
--------------

<div class="experience-container">
  <div class="experience-card">
      <div class="experience-logo" style="background:#B31B1B;color:#fff;font-size:11px;font-weight:700;display:flex;align-items:center;justify-content:center;text-align:center;line-height:1.15;">SJTU</div>
      <div class="experience-info">
          <strong>Shanghai Jiao Tong University</strong><br>
          <em>2024.09 - Present</em><br>
          M.S. student at <a href="http://www.cs.sjtu.edu.cn"><em>School of Computer Science</em></a>, advised by <a href="https://scholar.google.com/citations?user=yDEavdMAAAAJ&hl=zh-CN"><em>Xiaokang Yang</em></a> and <a href="https://daodaofr.github.io/"><em>Yichao Yan</em></a>
      </div>
  </div>

  <div class="experience-card">
      <div class="experience-logo" style="background:#003087;color:#fff;font-size:11px;font-weight:700;display:flex;align-items:center;justify-content:center;text-align:center;line-height:1.15;">SHU</div>
      <div class="experience-info">
          <strong>Shanghai University</strong><br>
          <em>B.E.</em><br>
          Received my bachelor's degree before joining SJTU
      </div>
  </div>
</div>
