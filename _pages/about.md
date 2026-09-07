---
permalink: /
layout: home
excerpt: "Research in LLM agents, information retrieval, and trustworthy AI."
description: "Xiaowei Qian, Ph.D. candidate at City University of Hong Kong. Research in LLM agents, information retrieval, and trustworthy AI."
redirect_from:
  - /about/
  - /about.html
---

<section class="profile-section" id="about-me" aria-labelledby="name">
  <div class="profile-text">
    <div class="name" id="name" role="heading" aria-level="1">Xiaowei Qian</div>
    <div class="pronunciation">Ph.D. Candidate, City University of Hong Kong</div>
    <div class="profile-email">{{ site.author.email }}</div>
    <div class="profile-links">
      <a href="mailto:{{ site.author.email }}">Email</a> /
      <a href="https://github.com/{{ site.author.github }}">GitHub</a> /
      <a href="{{ site.author.googlescholar }}">Google Scholar</a>
    </div>
  </div>
  <img class="profile-photo" src="{{ '/images/handsome.png' | relative_url }}" alt="Xiaowei Qian" width="160" height="160">
</section>

<section class="homepage-section biography-section" id="biography" aria-labelledby="biography-title">
  <h2 id="biography-title">Biography</h2>
  <p class="bio">I am a Ph.D. candidate at the City University of Hong Kong, supervised by Prof. <a href="https://zhaoxyai.github.io/">Xiangyu Zhao</a>. Previously, I received my B.Eng. from the University of Electronic Science and Technology of China (UESTC) and was a visiting student at Westlake University, supervised by Prof. <a href="https://tailin.org/">Tailin Wu</a>.</p>
  <p class="bio" id="research">My research interests include long-context and long-horizon LLM agents, information retrieval and deep research, and trustworthy AI, including safety, fairness, and robustness.</p>
</section>

<span id="-publications" class="legacy-anchor"></span>
<section class="homepage-section" id="publications" aria-labelledby="publications-title">
  <h2 id="publications-title">Selected Publications</h2>
  <p class="paper_rest">* Equal contribution</p>
  <ul class="publication-list">
    {% for paper in site.data.publications %}
    {% if paper.selected %}{% include arvid-paper.html %}{% endif %}
    {% endfor %}
  </ul>
  <a href="{{ '/publications.html' | relative_url }}" class="view-all">View all publications &rarr;</a>
</section>

<span id="background" class="legacy-anchor"></span>
<span id="-educations" class="legacy-anchor"></span>
<section class="homepage-section" id="education" aria-labelledby="education-title">
  <h2 id="education-title">Education</h2>
  <ul class="news-list">
    <li><span class="news-date">2025.09 – present</span><div>City University of Hong Kong, Ph.D. in Data Science</div></li>
    <li><span class="news-date">2024.07 – 2025.07</span><div>Westlake University, Visiting Student</div></li>
    <li><span class="news-date">2020.09 – 2024.06</span><div>University of Electronic Science and Technology of China, B.Eng. in Computer Science</div></li>
  </ul>
</section>

{% comment %}
<span id="-experiences" class="legacy-anchor"></span>
<span id="-internships" class="legacy-anchor"></span>
<section class="homepage-section" id="experience" aria-labelledby="experience-title">
  <h2 id="experience-title">Research experience</h2>
  <ul class="news-list">
        <li><span class="news-date">2024.07 – 2025.07</span><div><div>Westlake University · Visiting Student</div><div class="paper_rest"><a href="https://ai4s.lab.westlake.edu.cn/">AI for Scientific Simulation and Discovery Lab</a><br>Safe generative models · Prof. <a href="https://tailin.org/">Tailin Wu</a></div></div></li>
        <li><span class="news-date">2023.09 – 2024.02</span><div><div>Rensselaer Polytechnic Institute · Research Intern</div><div class="paper_rest"><a href="https://dami-lab.github.io/">Data Analytics and Machine Intelligence Lab</a><br>Trustworthy ML · Prof. <a href="https://scholar.google.com/citations?hl=en&amp;user=wf9TTOIAAAAJ">Yao Ma</a></div></div></li>
        <li><span class="news-date">2022.09 – 2023.09</span><div><div>UESTC · Research Intern</div><div class="paper_rest">Cognitive Computing and Intelligent Decision Lab<br>Graph representation learning · Prof. <a href="https://scholar.google.com/citations?user=T_yCaN4AAAAJ&amp;hl=en">Zhao Kang</a></div></div></li>
      </ul>
</section>
{% endcomment %}

<section class="homepage-section" id="service" aria-labelledby="service-title">
  <h2 id="service-title">Service</h2>
  <p><strong>Reviewer:</strong> KDD 2026, CVPR 2026, WWW 2026, AAAI 2027.</p>
</section>
