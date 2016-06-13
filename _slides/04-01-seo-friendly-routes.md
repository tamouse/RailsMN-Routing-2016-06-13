---
layout: slide
---

## Making SEO-Friendly Routes

Sometimes you want to make your routes more SEO-friendly, in that they
reflect the name of what you're trying to use.

The simplest way doesn't involve changing your **routes** file, at all.
Set the `to_param` class method in your model, and the path/URL helpers will automatically use it.
{:.fragment}

<div class="fragment">
<pre><code class="ruby">class Post < ActiveRecord::Base
  to_param :title
end

post_path(@post) # => "/posts/2-my-little-chthulu"</code></pre>
</div>
