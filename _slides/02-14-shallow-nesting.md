---
layout: slide
---

## Shallow Nesting

<div class="left-align">

A useful way to avoid deep nesting, yet keeping many of the benefits.

<pre><code class="ruby">resources :posts do
  resources :comments, only: [:index, :new, :create]
end
resources :comments, only: [:show, :edit, :update, :destroy]</code></pre>

Rails provides a shorthand for the above:

<pre><code class="ruby">resources :posts do
  resources :comments, shallow: true
end</code></pre>


</div>
