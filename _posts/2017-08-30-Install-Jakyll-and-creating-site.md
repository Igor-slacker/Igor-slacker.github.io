---
layout: post
title: "Створення сайту на Jekyll"
description: "Установка і налаштування Jekyll та створення сайту"
category: articles
tags: [Jekyll,website]
comments: false
---

Спроба запустити блог на Jekyll

#### Установка Jekyll

Для запуску і налаштування сайту на компʼютері потрібно встановити Jekyll. Для цього в терміналі даємо команду:

{% highlight bash %}
# gem install jekyll 
{% endhighlight %}

Потім скачуємо шаблон і наповнюємо його. Для запуску сервера Jekyll потрібно зайти в корінь сайту і дати команду:

{% highlight bash %}
$ jekyll serve
{% endhighlight %}

Для шаблона  White Paper, Jekyll видав якусь ругань відносно bundlerʼа. Довелося ще дещо зробити:

{% highlight bash %}
# gem install bundler
$ bundle install
$ bundle exec jekyll serve
{% endhighlight %}

Як виявилося це все описано в [README](https://github.com/vinitkumar/white-paper/blob/gh-pages/README.md#installation)

Після запуску сервера, в браузері переходимо на сайт за адресою:

<code>
  <a href="http://localhost:4000/">http://localhost:4000/</a>
</code>

#### Наповнення сайту

Щоб додати пост, ідемо до каталога _posts і створюємо фойл за типом:

{% highlight bash %}
YYYY-MM-DD-post-name.md
чи
YYYY-MM-DD-post-name.html
{% endhighlight %}

і наповнюємо його.