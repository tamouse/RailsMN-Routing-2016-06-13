---
layout: slide
---

## Rails Routing Resources

Rails standard routing by default <br>uses the concept of a resource.

<pre><code class="ruby">resources :photos</code></pre>

<div class="fragment">

Which creates 7 different routes:

| Verb + Path | Controller#Action |
|:------------|:------------------|
| GET /posts | posts#index |
| GET /posts/new | posts#new |
| POST /posts | posts#create |
| GET /posts/:id | posts#show |
| GET /posts/:id/edit | posts#edit |
| PUT /posts/:id | posts#update |
| DELETE /posts/:id | posts#destroy |
{: .small-table}

</div>
