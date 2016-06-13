---
layout: slide
---

## Restricting the Routes Created

Normally Rails creates the seven routes for the default controller actions
(`index`, `show`, `new`, `create`, `edit`, `update`, `destroy`) when you
specify a resource.

<div class="fragment">
You can restrict the routes by using the <br>keywords `only` and `except`

<pre><code class="ruby">resources :comments, only: [:index, :show]</code></pre>

|          Prefix | Verb   | URI Pattern                            | Controller#Action |
|----------------:|:-------|:---------------------------------------|:------------------|
|        comments | GET    | /comments(.:format)                    | comments#index    |
|                 | GET    | /comments/:id(.:format)                | comments#show     |
{:.small-table}
</div>
