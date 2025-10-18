---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

# Blog

Welcome to my blog! Here I share thoughts on research, data science, psychology, and academic life.

<!-- Search Bar -->
<input type="text" id="blog-search" placeholder="Search blog posts..." style="width:100%;padding:0.5em;margin-bottom:1em;">

<!-- Tag Filter Bar -->
<div id="tag-filter" style="margin-bottom:1em;"></div>

<!-- Featured Posts -->
<h2>Featured Posts</h2>
<div id="featured-posts">
  {% assign featured_posts = site.posts | where: "featured", true | sort: "date" | reverse %}
  {% for post in featured_posts limit:2 %}
    <div class="featured-post" style="display:flex;align-items:center;margin-bottom:1.5em;">
      {% if post.thumbnail %}
        <img src="/images/{{ post.thumbnail }}" alt="{{ post.title }}" style="width:120px;height:80px;object-fit:cover;margin-right:1em;border-radius:8px;">
      {% endif %}
      <div>
        <h3 style="margin:0;"><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p style="margin:0.2em 0 0.5em 0;"><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        <p>{{ post.excerpt }}</p>
        <a href="{{ post.url }}">Read more &rarr;</a>
      </div>
    </div>
  {% endfor %}
  
</div>

<hr/>

<!-- Blog Posts List -->
<div id="blog-posts-list">
  {% assign non_featured_posts = site.posts | where_exp: "post", "post.featured != true" %}
  {% for post in paginator.posts %}
    <div class="blog-post-preview" data-tags="{{ post.tags | join: ',' }}" style="display:flex;align-items:center;margin-bottom:1.5em;">
      {% if post.thumbnail %}
        <img src="/images/{{ post.thumbnail }}" alt="{{ post.title }}" style="width:100px;height:70px;object-fit:cover;margin-right:1em;border-radius:8px;">
      {% endif %}
      <div>
        <h3 style="margin:0;"><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p style="margin:0.2em 0 0.5em 0;"><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
        <p>{{ post.excerpt }}</p>
        <div class="post-tags">
          {% for tag in post.tags %}
            <span class="blog-tag" style="background:#eee;border-radius:4px;padding:2px 8px;margin-right:4px;font-size:0.9em;">{{ tag }}</span>
          {% endfor %}
        </div>
        <a href="{{ post.url }}">Read more &rarr;</a>
      </div>
    </div>
  {% endfor %}
</div>

<!-- Pagination -->
<div style="text-align:center;margin-top:2em;">
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">&larr; Newer Posts</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}" style="margin-left:2em;">Older Posts &rarr;</a>
  {% endif %}
</div>

<p><a href="/feed.xml">Subscribe via RSS</a></p>

<!-- Blog Search and Tag Filter Script -->
<script>
// Collect all tags
var allTags = Array.from(new Set(Array.from(document.querySelectorAll('.blog-post-preview')).flatMap(function(el){
  return (el.getAttribute('data-tags')||'').split(',');
}))).filter(Boolean);

// Render tag filter bar
var tagFilterDiv = document.getElementById('tag-filter');
allTags.forEach(function(tag){
  var btn = document.createElement('button');
  btn.textContent = tag;
  btn.className = 'blog-tag';
  btn.style = 'margin-right:6px;margin-bottom:6px;padding:4px 10px;border:none;background:#f0f0f0;border-radius:4px;cursor:pointer;';
  btn.onclick = function(){
    document.querySelectorAll('.blog-post-preview').forEach(function(post){
      post.style.display = post.getAttribute('data-tags').includes(tag) ? 'flex' : 'none';
    });
  };
  tagFilterDiv.appendChild(btn);
});
// Add "Show All" button
var showAllBtn = document.createElement('button');
showAllBtn.textContent = 'Show All';
showAllBtn.className = 'blog-tag';
showAllBtn.style = 'margin-right:6px;margin-bottom:6px;padding:4px 10px;border:none;background:#d0d0d0;border-radius:4px;cursor:pointer;';
showAllBtn.onclick = function(){
  document.querySelectorAll('.blog-post-preview').forEach(function(post){ post.style.display = 'flex'; });
};
tagFilterDiv.insertBefore(showAllBtn, tagFilterDiv.firstChild);

// Search functionality
var searchInput = document.getElementById('blog-search');
searchInput.addEventListener('input', function(){
  var q = this.value.toLowerCase();
  document.querySelectorAll('.blog-post-preview').forEach(function(post){
    var text = post.textContent.toLowerCase();
    post.style.display = text.includes(q) ? 'flex' : 'none';
  });
});
</script> 

