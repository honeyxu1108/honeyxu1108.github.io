---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<style>
    #news,
    #experience,
    #publications,
    #projects,
    #awards,
    #talks {
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

</style>
<html> 
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Fredericka+the+Great&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Homemade+Apple&display=swap');
        body {
            background-color:	 #FFFFFF;
            font-family: 'Arial Rounded MT Bold', 'Verdana', sans-serif;
            font-size: 15px;
        }
        .main-heading {
            font-family: 'Permanent Marker', cursive;
            text-align: center;
            color: #ca6f6f;
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
<h1 class="main-heading">Hi there <img src="images/Hi.gif" width="40px"> Welcome to my Homepage!</h1>
</body>
</html>

Hi! I am a junior (3rd-year) undergraduate student at Xidian University. 

My research interests include **MLLM**, **RL**, **Efficient AI** and other emerging areas in AI. I enjoy exploring diverse research directions and collaborating with researchers across different fields.

Feel free to reach out if you are interested in collaboration or potential opportunities.

News
---------------
<div class="news-box">
  <ul class="news-list">
    <li><span class="news-date">2026.05</span> 🎉🎉 I begin my internship at Alibaba Group.</li>
    <li><span class="news-date">2026.04</span> 🎉🎉 Two papers accepted to ACL 2026. (Not publicly available on arXiv yet due to visa-related clearance).</li>
    <li><span class="news-date">2026.02</span> 🎉🎉 One paper accepted to CVPR 2026. (Not publicly available on arXiv yet due to visa-related clearance).</li>
    <li><span class="news-date">2026.01</span> 🎉🎉 I begin my internship at TeleAI.</li>
    <li><span class="news-date">2025.08</span> 🎉🎉 One paper accepted to PRCV 2025.</li>
    <li><span class="news-date">2025.07</span> 🎉🎉 One paper accepted to ICCV 2025.</li>
    <li><span class="news-date">2024.10</span> 🎉🎉 I joined the HPC-AI Lab at NUS as a Research Assistant.</li>
  </ul>
</div>

Experience
--------------

<div class="experience-container">
  <div class="experience-card">
      <img src="images/Alibaba.png" alt="Alibaba logo" class="experience-logo">
      <div class="experience-info">
          <strong>Alibaba Group</strong><br>
          2026.05 - Present<br>
          MLLM Engineer Intern advised by <a href="https://liamding.cc/"><em>Liang Ding</em></a> and <a href="https://ethanscuter.github.io/"><em>Xintong Wang</em></a>
      </div>
  </div>


  
  <div class="experience-card">
      <img src="images/TeleAI.png" alt="TeleAI logo" class="experience-logo">
      <div class="experience-info">
          <strong>Institute of Artificial Intelligence of China Telecom</strong><br>
          2026.01 - 2026.03<br>
          Start My Journey in LLM
      </div>
  </div>

  <div class="experience-card">
      <img src="images/NUS.png" alt="NUS logo" class="experience-logo">
      <div class="experience-info">
          <strong>National University of Singapore</strong><br>
          2024.10 - 2025.10<br>
          Research Assistant at <a href="https://ai.comp.nus.edu.sg/"><em>HPC-AI Lab</em></a> advised by <a href="https://www.comp.nus.edu.sg/~youy/"><em>Yang You</em></a>, <a href="https://wangbo-zhao.github.io/"><em>Wangbo Zhao</em></a> and <a href="https://lancezpf.github.io/"><em>Pengfei Zhou</em></a>
      </div>
  </div>


  <div class="experience-card">
      <img src="images/XDU.png" alt="Xi'dian logo" class="experience-logo">
      <div class="experience-info">
          <strong>Xidian University</strong><br>
          2023.09 - Present<br>
          Rank 5/99, B.E at <a href="https://ste.xidian.edu.cn/"><em>School of Telecommunication Engineering</em></a> & Research Assistant advised by <a href="https://scholar.google.com/citations?user=k33uf2RE8nsC&hl=zh-CN&oi=ao"><em>Xiumei Wang</em></a>
      </div>
  </div>
  
</div>


Publications
--------------
<button class="pub-button active" onclick="filterPublications(event, 'all')">Core Publications</button>
<button class="pub-button" onclick="filterPublications(event, 'mllm')">MLLM</button>
<button class="pub-button" onclick="filterPublications(event, 'benchmark')">BenchMark</button>

(* equal contribution · &dagger; corresponding author · &Dagger; project leader)

<div class="publication-card" data-category="mllm benchmark"> 
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;"> 
      <img src="images/GroupToM.png" alt="wog" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;"> 
    </div> 
    <div>
      <strong>GroupToM-Bench: Benchmarking Group Theory of Mind and Nonlinear Social Emergence in MLLMs</strong><br>
      <i style="font-size: 13px;">
        <a href="https://wd7ang.github.io" target="_blank"><strong>Weidong Tang</strong></a>, 
        Jierui Li,
        Yueling Hou, 
        Zihan Mei, 
        Zhigang Tian, 
        Weicheng Jiao, 
        Can Zhang, 
        Xinyan Wan, 
        <a href="https://jerryliang24.github.io/" target="_blank">Zhiyuan Liang</a>, 
        <a href="https://lancezpf.github.io/" target="_blank">Pengfei Zhou&dagger;</a>,
        <a href="https://www.comp.nus.edu.sg/~youy/" target="_blank">Yang You</a>, 
        <a href="https://wangbo-zhao.github.io/" target="_blank">Wangbo Zhao&dagger;</a>
      </i><br> 
      We propose GroupToM-Bench and show that current models fail at nonlinear group reasoning despite strong individual-level ToM, exposing a clear group cognitive gap. 
      <br> 
      <b><i style="color:#83a1c7;">ACL 2026 Oral &nbsp;
      </i></b> 
      <a href=""><em>[arXiv]</em></a> 
      <a href=""><em>[code]</em></a> 
    </div>
  </div> 
</div>


<div class="publication-card" data-category="mllm benchmark"> 
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;"> 
      <img src="images/MagicBench.png" alt="wog" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;"> 
    </div> 
    <div>
      <strong>MagicBench: Diagnosing Visual Agency Loss and Semantic Dependency in Multimodal LLMs</strong><br>
      <i style="font-size: 13px;">
        Tang Da Huang,
        <a href="https://wd7ang.github.io" target="_blank"><strong>Weidong Tang&Dagger;</strong></a>, 
        Wen Qi Xu,
        Xianpeng Guo&dagger;
      </i><br> 
      The authors introduce MagicBench, a video dataset of magic tricks, to test if Multimodal LLMs actually rely on visual physics or if they are overly dependent on language narratives (which, in magic tricks, are deliberately deceptive).
      <br> 
      <b><i style="color:#83a1c7;">ACL 2026 &nbsp;
      </i></b> 
      <a href=""><em>[arXiv]</em></a> 
      <a href=""><em>[code]</em></a> 
    </div>
  </div> 
</div>


<div class="publication-card" data-category="mllm benchmark"> 
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;"> 
      <img src="images/RDS.png" alt="wog" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;"> 
    </div> 
    <div>
      <strong>Efficient Video Object Segmentation and Tracking with Recurrent Dynamic Submodel</strong><br>
      <i style="font-size: 13px;">
        <a href="https://wd7ang.github.io" target="_blank"><strong>Weidong Tang</strong></a>, 
        <a href="https://jerryliang24.github.io/" target="_blank">Zhiyuan Liang</a>, 
        Xinyan Wan, 
        <a href="https://scholar.google.com.hk/citations?user=W9HbDoYAAAAJ&hl=en" target="_blank">Chen Zhu</a>, 
        <a href="https://scholar.google.com.hk/citations?user=qNWDwOcAAAAJ&hl=en" target="_blank">Zhaopan Xu</a>, 
        <a href="https://lancezpf.github.io/" target="_blank">Pengfei Zhou</a>&dagger;,
        Yan Song,
        <a href="https://www.comp.nus.edu.sg/~youy/" target="_blank">Yang You</a>, 
        <a href="https://wangbo-zhao.github.io/" target="_blank">Wangbo Zhao&dagger;</a>
      </i><br> 
      Proposed a Recurrent Dynamic Submodel for efficient Video Object Segmentation and Tracking. By integrating temporal-prior-guided global dynamic routing and Importance-aware LoRA, it achieves an optimal trade-off between performance and speed using minimal trainable parameters and training data.
      <br> 
      <b><i style="color:#83a1c7;">CVPR 2026 &nbsp;
      </i></b> 
      <a href=""><em>[arXiv]</em></a> 
      <a href=""><em>[code]</em></a> 
    </div>
  </div> 
</div>


<div class="publication-card" data-category="mllm benchmark"> 
  <div style="display: flex; align-items: center;">
    <div class="pub-media-rotator" data-interval="4000" style="position: relative; width: 320px; height: 180px; margin-right: 20px; border-radius: 8px; overflow: hidden; flex: 0 0 auto;"> 
      <img src="images/var-scaling.png" alt="wog" style="width: 320px; height: 180px; object-fit: contain; display: block; margin: 0 auto;"> 
    </div> 
    <div>
      <strong>Inference-Time Scaling for Visual AutoRegressive modeling by Searching Representative Samples</strong><br>
      <i style="font-size: 13px;">
        <a href="https://wd7ang.github.io" target="_blank"><strong>Weidong Tang</strong></a>, 
        Xinyan Wan,
        <a href="https://scholar.google.com/citations?user=k33uf2RE8nsC&hl=zh-CN&oi=ao" target="_blank">Xiumei Wang&dagger;</a>
      </i><br> 
      Explored inference-time scaling in discrete spaces by mapping them to continuous spaces to obtain density distributions, thereby optimizing the sampling of early coarse-scale features.
      <br> 
      <b><i style="color:#83a1c7;">PRCV 2025 &nbsp;
      </i></b> 
      <a href=""><em>[arXiv]</em></a> 
      <a href=""><em>[code]</em></a> 
    </div>
  </div> 
</div>



<script src="assets/js/show_publications.js"></script>
<script src="assets/js/pub_media_rotator.js"></script>


Projects
--------
<div class="project-card" data-category="project"> 
  <div style="display: flex; align-items: center;"> 
    <div class="pub-media-rotator"
         style="position: relative; width: 240px; height: 140px; 
                margin-right: 20px; border-radius: 8px; overflow: hidden; 
                flex: 0 0 auto; display: flex; justify-content: center; align-items: center;">
      <img src="images/GroupToM.png" alt="ManiUniCon"
           style="max-width: 100%; max-height: 100%; object-fit: contain;">
    </div>
    <div> 
      <strong>ManiUniCon: A Unified Control Interface for Robotic Manipulation</strong><br>
      <i style="font-size: 13px;">
        Universal-Control Team
      </i><br>
      ManiUniCon is a comprehensive, multi-process robotics control framework designed for robotic manipulation tasks. It provides a unified interface for controlling various robot arms, integrating sensors, and executing policies in real-time. 
      <br> 
      <b><i style="color:#83a1c7;">Project &nbsp;</i></b> 
      <a href="https://github.com/Universal-Control/ManiUniCon"><em>[code]</em></a> 
    </div>
  </div> 
</div>


Awards
--------
- Xiaomi Outstanding Scholarship 2025
- National Scholarship 2025
- Outstanding Student, Xidian University, 2025


Talks
--------
- [2026/03] Invited to [Talk on RoboTion](http://xhslink.com/o/74L1xM2Vw2f) about WoG.
- [2025/12] Invited to [Talk on NICE seminar](https://www.bilibili.com/video/BV1utBrBfED4?spm_id_from=333.788.videopod.episodes&p=9) about Imitation Learning
- [2025/12] Invited to [Talk on RL China](https://b23.tv/We6FLQh) about DSPv2
- [2025/10] Invited to [Talk on 3D视觉工坊](https://b23.tv/PvLKNR1) about DSP and DSPv2
