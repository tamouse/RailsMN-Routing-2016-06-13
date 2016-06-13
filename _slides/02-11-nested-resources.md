---
layout: slide
---

## Nested Resources

<div class="left-align">

Resources are logically nested, with children and parents. In our classic model, Comments and the children of Posts.

<pre><code class="ruby">class Post < ActiveRecord::Base
  has_many :comments
end

class Comment < ActiveRecord::Base
  belongs_to :post
end</code></pre>

Nesting routes captures this relationship:

<pre><code class="ruby">resources :posts do
  resources :comments
end</code></pre>

</div>
