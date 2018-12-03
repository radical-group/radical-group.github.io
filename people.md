---
title: People
permalink: /people/
---

{% assign people_sorted = site.people|sort: 'joined' %}
{% assign people_array = "pi|researcher|phd|ms|undergrad|visiting" | split: "|" %}


<div class="content list people">
{% for item in people_array %}
  {% for profile in people_sorted %}
    {% if profile.position contains item %}
    <div class="list-item-people">
      <p class="list-post-title">
        {% if profile.avatar %}
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="{{site.baseurl}}/images/people/{{profile.avatar}}" alt="{{profile.name}} photo"></a>
        {% else %}
        <a href="{{ site.baseurl }}{{ profile.url }}"><img width="200" src="http://evansheline.com/wp-content/uploads/2011/02/facebook-Storm-Trooper.jpg"></a>
        {% endif %}
        <a class="name" href="{{ site.baseurl }}{{ profile.url }}" style="float: middle">{{ profile.name }}</a><br>
        <a class="name" href="{{ site.baseurl }}{{ profile.url }}" style="float: middle">{{ profile.title }}</a>
      </p>
    </div>    
    {% endif %}
  {% endfor %}
  {% endfor %}
</div>
<hr>

<h3>Alumni</h3>
<dl style="font-size:0.7rem;">
<li>Ming Tai Ha</li>
<li>Ole Weidner</li>
<li>Franklin Bettencourt</li>
<li>Alessio Angius</li>
<li>Nivetha Balasamy</li>
<li>Antons Treikalis</li>
<li>Nikhil Shenoy</li>
<li>Suvigya Tripathi</li>
<li>Dinesh Ganapathi</li>
<li>Vishal Shah</li>
<li>Anjani Bhargavi</li>
<li>Abhinav Thota</li>
<li>Pradeep Mantha</li>
<li>Sharath Maddineni</li>
<li>Chris Miceli</li>
<li>Michael Miceli</li>
<li>Hartmut Kaiser)</li>
<li>Ashley Zebrowski</li>
<li>Aikaterina Stamou</li>
</dl>
