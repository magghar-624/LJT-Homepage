---
permalink: /
title: "Junteng Liu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD candidate at the [HKUST NLP Group](https://nlphug.com/), supervised by [Professor Junxian He](https://jxhe.github.io/). I graduated from [Shanghai Jiao Tong University (SJTU)](https://www.sjtu.edu.cn/) in June 2024. My research focuses on natural language processing and machine learning, with specific interests in LLM Reasoning and Reinforcement Learning, Hallucination in Vision-Language Models (VLM), and LLM Truthfulness and Interpretability.

Education
======
- **Ph.D. in Computer Science**, Hong Kong University of Science and Technology, 2024-Present
- **B.Eng.**, Shanghai Jiao Tong University, 2020-2024

Research Experience
======
- **Research Intern**, MINIMAX, February 2025 - Present
- **Research Intern**, Tencent WXG (Advisor: Zifei Shan), June 2024 - September 2024
- **Research Intern**, Shanghai AI Lab (Advisor: Prof. Yu Cheng), June 2023 - December 2023

Honors and Awards
======
- Zhiyuan Honor Scholarship, Shanghai Jiao Tong University

Publications
======
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

Skills
======
- Natural Language Processing
- Machine Learning
- LLM Reasoning and Reinforcement Learning
- Hallucination in Vision-Language Models (VLM)
- LLM Truthfulness and Interpretability

Contact
======
- **Email**: jliugi@connect.ust.hk
- **GitHub**: [Vicent0205](https://github.com/Vicent0205)
- **Google Scholar**: [Profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
- **X (Twitter)**: [@junteng88716710](https://twitter.com/junteng88716710)
