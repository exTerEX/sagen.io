# Sagen.io

Source code for my own website using jekyll and docker. The site is designed after [poole/lanyon](https://github.com/poole/lanyon) and [poole/poole](https://github.com/poole/poole). The source code in this repository is not intended to be reused and is stripped for coloring templates and functionallity I don't need for my website. If you enjoy the design use `lanyon's` design as a template and use,

```html
<div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ post.url | absolute_url }}"> {{ post.title }} </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    <p>{{ post.content | truncatewords: 90 }}</p>
  </div>
  {% endfor %}
</div>
```

in your `index.html` instead of `poole/lanyon's` code block if you want truncate support.

## License

This repository is distrbuted under `MIT`. For more information see [LICENSE](LICENSE).
