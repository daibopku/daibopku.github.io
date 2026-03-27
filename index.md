---
layout: default
title: Bo Dai
---

## Biography
{:#biography}

Dr. Bo Dai received his B.S. and Ph.D. degrees in Physics from Peking University. He later transitioned to artificial intelligence as a postdoctoral researcher at the [School of Intelligence Science and Technology](http://www.cis.pku.edu.cn/), Peking University, advised by [Prof. Song-Chun Zhu](http://www.stat.ucla.edu/~sczhu/).

His research bridges cognitive science and artificial intelligence, focusing on two main directions: (1) building machines that can learn abstract representations, causal relations, and physical commonsense directly from physical environments through the lens of intuitive physics, and (2) evaluating multimodal large language model-based embodied agents in high-dimensional semantic action spaces by constructing comprehensive test scenarios.

Dr. Dai is currently a research scientist at the [Institute for Artificial Intelligence, Peking University](https://www.bigai.ai/) (Beijing Institute for General Artificial Intelligence, BIGAI), where he leads the embodied general AI testing initiatives at the General Agent Center.

<!-- 添加 CV 链接时请取消注释下行 -->
<!-- [<u>CV</u>](files/cv.pdf) -->

---

## Topics
{:#topics}

<div class="topics">
  <span class="topic-tag">Intuitive Physics</span>
  <span class="topic-tag">Embodied AI</span>
  <span class="topic-tag">Cognitive Science</span>
  <span class="topic-tag">Physical Commonsense</span>
  <span class="topic-tag">Causal Reasoning</span>
  <span class="topic-tag">LLM Evaluation</span>
  <span class="topic-tag">Multi-modal Learning</span>
</div>

---

## Publications
{:#publications}

<!-- 论文列表 - 按时间倒序排列 -->

{% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
{% for pub in sorted_pubs %}
<div class="pub-entry">
  {% if pub.thumbnail %}
  <div class="pub-thumbnail">
    <a href="{{ pub.url | relative_url }}">
      {% assign thumb_ext = pub.thumbnail | split: '.' | last | downcase %}
      {% if thumb_ext == 'pdf' %}
        <iframe src="{{ pub.thumbnail | relative_url }}#toolbar=0&navpanes=0&page=1&zoom=fit" frameborder="0" scrolling="no"></iframe>
      {% else %}
        <img src="{{ pub.thumbnail | relative_url }}" alt="{{ pub.title }}">
      {% endif %}
    </a>
  </div>
  {% endif %}
  <div class="pub-info">
    <div class="pub-entry-title">
      <a href="{{ pub.url | relative_url }}">{{ pub.title }}</a>
    </div>
    <div class="pub-entry-authors">{{ pub.authors }}</div>
    <div class="pub-entry-venue">{{ pub.venue }}</div>
    <div class="pub-entry-links">
      {% if pub.pdf %}[<u>PDF</u>]({{ pub.pdf }}){% endif %}
      {% if pub.arxiv %}[<u>arXiv</u>]({{ pub.arxiv }}){% endif %}
      {% if pub.code %}[<u>Code</u>]({{ pub.code }}){% endif %}
      {% if pub.dataset %}[<u>Dataset</u>]({{ pub.dataset }}){% endif %}
      {% if pub.project %}[<u>Project</u>]({{ pub.project }}){% endif %}
      {% if pub.video %}[<u>Video</u>]({{ pub.video }}){% endif %}
      {% if pub.poster %}[<u>Poster</u>]({{ pub.poster }}){% endif %}
      {% if pub.slides %}[<u>Slides</u>]({{ pub.slides }}){% endif %}
      {% if pub.doi %}[<u>DOI</u>]({{ pub.doi }}){% endif %}
    </div>
  </div>
</div>
{% endfor %}

---

## Pre-Print
{:#preprints}

<!-- 在这里添加预印本论文 -->

<!-- 示例：
<div class="pub-entry">
  <div class="pub-entry-title">Paper Title: Subtitle</div>
  <div class="pub-entry-authors">Author One, <u>Bo Dai</u>, Author Three</div>
  <div class="pub-entry-links">
    [<u>PDF</u>](链接) [<u>arXiv</u>](链接) [<u>Code</u>](链接) [<u>Dataset</u>](链接)
  </div>
</div>
-->
