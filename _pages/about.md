---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

Hello! I'm Haotian (Eric) Xia (夏浩天), a second-year Ph.D. student in Computer Science at Rice University, advised by Prof. [Hanjie Chen](https://hanjiechen.github.io/) in the Chili Lab. I work on **multimodal understanding and reasoning**: building vision-language models that find the evidence that matters in images and video, then reason over it accurately and efficiently.

I earned my M.S. in Statistics at the University of California, Irvine, advised by Prof. [Weining Shen](https://faculty.sites.uci.edu/weinings/), and my B.S. in Computer Science with Distinction at the University of California, Santa Barbara, advised by Prof. [Yuan-Fang Wang](https://engineering.ucsb.edu/people/yuan-fang-wang) and Prof. [Linda Petzold](https://engineering.ucsb.edu/people/linda-petzold).

## Research

<div class="focus-grid">
  <section class="focus">
    <h3>Multimodal understanding</h3>
    <p>Grounding language in visual evidence across images and long or streaming video.</p>
    <p class="focus__papers"><a href="https://arxiv.org/abs/2608.04124">DyLaR</a> · <a href="https://arxiv.org/abs/2511.06499">SportR</a></p>
  </section>
  <section class="focus">
    <h3>Multimodal reasoning</h3>
    <p>Latent and adaptive reasoning, post-trained with reinforcement learning, for both accuracy and inference efficiency.</p>
    <p class="focus__papers"><a href="https://arxiv.org/abs/2608.04124">DyLaR</a> · <a href="https://arxiv.org/abs/2511.12908">DeepSport</a></p>
  </section>
  <section class="focus">
    <h3>AI for sports and beyond</h3>
    <p>Benchmarks that test rules, tactics and physical decision-making, with sports as a demanding real-world testbed.</p>
    <p class="focus__papers"><a href="https://arxiv.org/abs/2410.08474">SPORTU</a> · <a href="https://arxiv.org/abs/2607.14616">SportD</a> · <a href="https://arxiv.org/abs/2508.09641">VisFinEval</a></p>
  </section>
</div>

## News

<ul class="news">
{% for item in site.data.news %}<li><span class="news__date">{{ item.date }}</span><span class="news__text">{{ item.text }}</span></li>
{% endfor %}</ul>

## Selected Publications

<p class="section-note"><sup>*</sup> Equal contribution. <a href="{{ base_path }}/publications/">All publications</a></p>

<ul class="pub-list">
{% for p in site.data.publications %}{% if p.selected %}{% include pub-item.html pub=p card=true %}{% endif %}{% endfor %}
</ul>

## Beyond Research

<div class="beyond">
  <div class="beyond__text">
    <p>I started playing volleyball at the age of seven and later competed as an NCAA Division I student-athlete on an athletic scholarship with the nationally top-3-ranked UCSB Men's Volleyball team, winning the 2021 Big West Conference title. I am also recognized as a National Level Athlete (国家一级运动员) in China.</p>
    <p>If you'd like to talk about multimodal reasoning or sports analytics, feel free to <a href="mailto:{{ site.author.email }}">email me</a>.</p>
  </div>
  <img class="beyond__photo" src="{{ base_path }}/images/voll.jpg" alt="Haotian Xia going up for a spike in a volleyball match" loading="lazy">
</div>
