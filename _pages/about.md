---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Staff Research Scientist and Tech Lead at Google Research, where I specialize in Artificial Intelligence. My work is centered on establishing the factuality of Large Language Models, with a specific focus on Gemini. My research spans the entire model development lifecycle, developing pre-training and Reinforcement Learning methods that endow LLMs with profound knowledge and minimize hallucinations.

I earned my PhD in Natural Language Processing from Tel Aviv University as a recipient of the [Google PhD Fellowship](https://ai.googleblog.com/2018/04/announcing-2018-google-phd-fellows-for.html). During my doctoral studies, I completed three research internships at Google. Prior to my PhD, I was a Research Staff Member at IBM Research, where I worked on Deep Learning architectures for NLP. My research has been recognized with an [INLG Best Paper Award](https://aclanthology.org/W17-3541.pdf) and a [NAACL Best Resource Paper Award](https://arxiv.org/pdf/1811.00937).

## 📜 Publications

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
      <td class="tg-wk8r"><strong>{{ pub.venue }}</strong></td>
      <td class="tg-oe15">
        <strong>{{ pub.title }}</strong>
        
        {% if pub.star %}
          <img src="{{ "/images/trophy.png" | relative_url }}" alt="Star" style="width: auto; height: 18px;"/>
        {% endif %}

        {% if pub.award %}
          <span style="color:#800000;">{{ pub.award }}</span>
        {% endif %}

        {% if pub.media %}
          <span style="color:#800000;">{{ pub.media }}</span>
        {% endif %}

        <br>{{ pub.authors }}
        <span style="display: block; margin-bottom: -13px;"></span> <br> 
        
        <a href="{{ pub.pdf }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Paper-80000f" alt="PDF" style="width: auto; height: 20px;"/>
        </a>
        
        {% if pub.github %}
        <a href="{{ pub.github }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Code-004f80" alt="GitHub Repository" style="width: auto; height: 20px;"/>
        </a>
        {% endif %}

        {% if pub.project %}
        <a href="{{ pub.project }}" target="_blank" rel="noopener noreferrer">
          <img src="https://img.shields.io/badge/Website-228B22" alt="Project page" style="width: auto; height: 20px;"/>
        </a>
        {% endif %}
      </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
