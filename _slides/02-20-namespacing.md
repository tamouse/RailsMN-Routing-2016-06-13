---
layout: slide
---

## Namespacing

The concept of "namespacing" goes across Rails in several ways.
Namespacing routes will allow you to place a resource under a common path,
and is often used in conjunction with namespaced controllers.

<div class="fragment">

In a namespaced controller, you'll have a parent module and the controller class:

<pre><code class="ruby">class Admin::UsersController < Admin::BaseController</code></pre>

In routing, you'd follow suit:

<pre><code class="ruby">namespace :admin do
  resources :users
end</code></pre>

</div>
