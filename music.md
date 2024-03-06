---
title: Music
layout: posts
sub_heading: ''
description: 
publish_date: '2024-03-06T03:00:00.000+00:00'
menu:
  navigation:
    identifier: _music
    weight: 

---
<section class="news">
   <div class="container pure-g">
        <div class="pure-u-1">
            <div class="content content-narrow">
                <h2>Latest Music Posts</h2>
                <ul class="posts">
                    {% assign musicPosts = site.posts | where: 'categories', 'music' %}
                    {% for post in musicPosts %}
                    <li>
                        <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
                        <date>{{ post.date | date_to_string }}</date>
                        <date>{{ post.sub_heading }}</date>
                    </li>
                    {% endfor %}
                </ul>
            </div>
        </div>
    </div>
</section>

