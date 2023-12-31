---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 한양대에 온 것을 환영해요 🦁

> 🤕변경되었거나 잘못된 정보가 있다면 댓글로 알려주세요🤕

> 추후에 수정이 안될 경우가 있을땐 알려드릴게요
> (그 전에 에타 외의 다른 방법을 사용해 정리할 예정이에요)

새해 D-1 인데 할게 없어서 만들어 봤어요


- [채팅방 홍보 목록](hyu_welcome_chat)

[[hyumemo]]

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Take a look at <span style="font-weight: bold">[[Your first note]]</span> to get started on your exploration.
</p>

This digital garden template is free, open-source, and [available on GitHub here](https://github.com/maximevaillancourt/digital-garden-jekyll-template).

The easiest way to get started is to read this [step-by-step guide explaining how to set this up from scratch](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll).

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
