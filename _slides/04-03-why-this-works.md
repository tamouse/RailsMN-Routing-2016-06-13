---
layout: slide
---

## Why this works

The reason this works is pretty simple, and a little stupid: When Rails runs the `.find(id)` method, it first runs `.to_i` on the id. Since the actual id number is the first thing in the parameterized "slug", it can determine the id:

<pre><code class="ruby">"2-my-little-chthulu".to_i # => 2</code></pre>

<div class="fragment">
So:
{:.left-align}

<pre><code class="ruby"># .. in PostsController#set_post:
@post = Post.find(params[:id])
# => Post.find("2-my-little-chthulu")
# => Post.find(2)</code></pre>
</div>
