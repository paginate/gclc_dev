---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<div class="home">
    <section class="main-slides">
        <article class="slide">
            <iframe class="slideshow-iframe" src="{{site.baseurl}}/images/index_slider1.html"></iframe>
            <div class="sub-slideshow">
            <h1>{{ slide.title }}</h1>
            </div>
        </article>
    </section>

  <h2 class="page-heading">Welcome to Grace Chinese Lutheran Church</h2>
  
  <div class="homepageTextBox">Sunday Worship Service at 11:00 am!</div>
    
  <h3>Latest News</h3>
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h4>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
        </h4>
      </li>
    {% endfor %}
  </ul>

</div>
