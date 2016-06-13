---
layout: slide
---

## Additional RESTful Actions

You can add more actions to a resource by adding routes to the collection or individual members.

<pre><code class="ruby">resources :posts do
  resources :comments, shallow: true
  collection do
    get 'search'
  end
  member do
    get 'review'
  end
end</code></pre>

|          Prefix | Verb   | URI Pattern                            | Controller#Action |
|----------------:|:-------|:---------------------------------------|:------------------|
|    search_posts | GET    | /posts/search(.:format)                | posts#search      |
|     review_post | GET    | /posts/:id/review(.:format)            | posts#review      |
{:.small-table}
