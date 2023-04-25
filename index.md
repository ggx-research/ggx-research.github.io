---
layout: page
title: About
---

This page contains the unofficial webpage for our Grenoble GraphiX (GGX) Research team. Now at Intel, previously at Unity.

<h3>Team</h3>
{% assign members = site.data.members | where: "center", "ggx" %}
<div style="display:flex; width:100%; flex-wrap:wrap">
{% for people in members %}
<div style="display:flex; width:45%; max-width: 45%; margin:1% 1% 1% 1%; border: 1px solid black; padding:1%; border-radius: 5px; background-color: rgb(240,240,240); box-shadow: 0 3px 8px 0 rgba(0,0,0,0.03);">
    <div class="people-picture" style="margin-right:2%">
        {% if people.photo %}
        <img width="92px" height="92px" style="max-width:none; width:90px; height:90px; overflow: hidden; border: solid 1px black;" src="{{ people.photo | prepend: site.baseurl }}" />
        {% else %}
        <img width="92px" height="92px" style="max-width:none; width:90px; height:90px; overflow: hidden;" src="{{ site.baseurl }}/images/people/default.svg" />
        {% endif %}
    </div>
    <div style="display:flex; flex-direction:column; justify-content:space-between;" class="people-infos">
        <div>
            <div>
                <span style="font-weight: 600;">
                {{ people.name }}
                </span><br />
                <span>
                {{ people.title }}
                </span>
                {% if people.email %}
                {% endif %}
            </div>

            {% if people.topics %}
            <div style="font-style: italic;">
                <span>{{ people.topics }}</span>
            </div>
            {% endif %}
        </div>

        <br />
        <div>
            {% if people.url %}
            <a class="member_website" href="{{ people.url }}">&nbsp;website</a>
            {% endif %}
            {% if people.email and people.url %}
            &nbsp;-&nbsp;
            {% endif %}
            {% if people.email %}
            <a class="member_email" href="mailto:{{ people.email }}">&nbsp;email </a>
            {% endif %}
        </div>
    </div>
</div>
{% endfor %}
</div>
<br /> <br />

<h3>Alumni</h3>
{% assign members = site.data.members | where: "center", "alumni" %}
<div style="display:flex; width:100%; flex-wrap:wrap">
{% for people in members %}
<div style="display:flex; width:45%; max-width: 45%; margin:1% 1% 1% 1%; border: 1px solid black; padding:1%; border-radius: 5px; background-color: rgb(240,240,240); box-shadow: 0 3px 8px 0 rgba(0,0,0,0.03); opacity: 0.5;">
    <div class="people-picture" style="margin-right:2%">
        {% if people.photo %}
        <img width="92px" height="92px" style="max-width:none; width:90px; height:90px; overflow: hidden; border: solid 1px black;" src="{{ people.photo | prepend: site.baseurl }}" />
        {% else %}
        <img width="92px" height="92px" style="max-width:none; width:90px; height:90px; overflow: hidden;" src="{{ site.baseurl }}/images/people/default.svg" />
        {% endif %}
    </div>
    <div style="display:flex; flex-direction:column; justify-content:space-between;" class="people-infos">
        <div>
            <div>
                <span style="font-weight: 600;">
                {{ people.name }}
                </span><br />
                <span>
                {{ people.title }}
                </span>
                {% if people.email %}
                {% endif %}
            </div>

            {% if people.topics %}
            <div style="font-style: italic;">
                <span>{{ people.topics }}</span>
            </div>
            {% endif %}
        </div>

        <br />
        <div>
            {% if people.url %}
            <a class="member_website" href="{{ people.url }}">&nbsp;website</a>
            {% endif %}
            {% if people.email and people.url %}
            &nbsp;-&nbsp;
            {% endif %}
            {% if people.email %}
            <a class="member_email" href="mailto:{{ people.email }}">&nbsp;email </a>
            {% endif %}
        </div>
    </div>
</div>
{% endfor %}
</div>
