---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Staff Research Scientist specializing in Artificial Intelligence. My current work at Google focuses on enhancing the factuality of Large Language Models (LLMs), with a specific emphasis on the Gemini models. My research spans the entire model development lifecycle, from foundational pre-training to targeted post-training techniques aimed at improving reliability and accuracy.

I hold a PhD in Natural Language Processing (NLP) from Tel Aviv University, where my doctoral studies were supported by the prestigious Google PhD Fellowship. Prior to my current role, I gained foundational experience as a Research Staff Member at IBM Research and further honed my skills through three research internships at Google. My contributions to the field have been recognized with a Best Resource Paper Award at NAACL 2019 and a Best Paper Award at INLG 2017.

# Publications

---
<style type="text/css">
  .tg  {border-collapse:collapse;border-spacing:0;}
  .tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px; overflow:hidden;padding:10px 5px;word-break:normal;}
  .tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px; font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
  .tg .tg-oe15{background-color:#ffffff;border-color:#ffffff;text-align:left;vertical-align:top}
  .tg .tg-wk8r{background-color:#ffffff;border-color:#ffffff;text-align:center;vertical-align:top}
</style>

<table class="tg">
  <tbody>
    {% for pub in site.data.publications %}
    <tr>
      <td class="tg-wk8r">{{ pub.venue }}</td>
      <td class="tg-oe15">
        {{ pub.title }}
        
        {% if pub.star %}
          <img src="trophy.png" alt="Star" style="width: auto; height: 18px;"/>
        {% endif %}

        {% if pub.award %}
          <span style="color:#800000;">{{ pub.award }}</span>
        {% endif %}

        {% if pub.media %}
          <span style="color:#800000;">{{ pub.media }}</span>
        {% endif %}

        <br>{{ pub.authors }}
        <span style="display: block; margin-bottom: -13px;"></span> <br> 
        
        <a href="{{ pub.pdf }}">
          <img src="https://img.shields.io/badge/PDF-80000f" alt="PDF" style="width: auto; height: 20px;"/>
        </a>
        
        {% if pub.github %}
        <a href="{{ pub.github }}">
          <img src="https://img.shields.io/badge/GitHub-004f80" alt="GitHub Repository" style="width: auto; height: 20px;"/>
        </a>
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
