---
layout: menu_page
title: Portfolio
permalink: /portfolio/
# image: ../images/menu/photo_portfolio.jpg
---

<meta charset="UTF-8">

<!-- <img src="../images/menu/RajeshProfilePic2.jpg" style="width:0%; height:0%; top:0; bottom:0"> -->

<div class="container">
  <div style="width:100%;height:0; padding-top:50%; overflow: hidden; position:relative;">
    <img src="../images/menu/photo_portfolio.jpg" style="width:100%; opacity:0.8; position:absolute; top:0; left:0">
  </div>  
  <div class="content" style="position:absolute;">
    <h1>Portfolio</h1>
    <p><span class="cover-desc">My portfolio showcases a variety of machine learning projects spanning Generative AI, Large Language Models (LLMs), Latural Language Processing (NLP), Recommendation Systems, Computer Vision and applications with tabular data. To explore more of my work, you can visit my <a href="https://github.com/vrajeshtrichy">GitHub page</a>, download my <a href="https://vrajeshtrichy.github.io/website/cv.pdf">Resume</a> or navigate to <a href="https://vrajeshtrichy.github.io/website/about/">about</a> page.</span></p>
  </div>
</div>

<p><span class="page-desc">My portfolio showcases a variety of machine learning projects spanning Generative AI, Large Language Models (LLMs), Natural Language Processing (NLP), Recommendation Systems, Computer Vision and applications with tabular data. To explore more of my work, you can visit my <a href="https://github.com/vrajeshtrichy">GitHub page</a>, download my <a href="https://vrajeshtrichy.github.io/website/cv.pdf">Resume</a> or navigate to <a href="https://vrajeshtrichy.github.io/website/about/">about</a> page.</span></p>


<!----------------------------------------------------------------------------->

<script src="{{ base.url | prepend: site.url }}/assets/js/read_more.js"></script>
<script src="{{ base.url | prepend: site.url }}/assets/js/accordion.js"></script>

<hr style="height:1px; visibility:hidden;" />

<div style="font-size: 100%;">

  <p>My portfolio features the following projects:</p>

  {% assign posts = site.posts %}

  <ul style="margin-top: -10px;">
  {%- if posts.size > 0 -%}
    {%- for post in posts -%}
    <li>🤖<a href="#{{ post.project_id}}">{{ post.title}} </a></li>
    {%- endfor -%}
  {%- endif -%}
  </ul>

  <p>Click "Project Title" to see more project details. Follow GitHub links for code and documentation.</p>

</div>

<!----------------------------------------------------------------------------->




{%- if posts.size > 0 -%}
  {%- if page.list_title -%}
    <h2 class="post-list-heading">{{ page.list_title }}</h2>
  {%- endif -%}
  <ul class="post-list">
    {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    {%- for post in posts -%}
    <li>
      <a id='{{ post.project_id }}'></a>
      {%- if site.show_image -%}
          {%- include post_list_image_card.html -%}
      {% else %}
          {%- include post_list.html -%}
      {%- endif -%}
    </li>
    {%- endfor -%}
  </ul>
{%- endif -%}