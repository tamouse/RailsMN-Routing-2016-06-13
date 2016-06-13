---
layout: slide
---

## Routing Matches

If the "/posts/2-my-little-chthulu" URL path is issued with a GET HTTP verb, it would match:

| Prefix | Verb | URI Pattern | Controller#Action |
|-------:|:-----|:------------|:------------------|
| post   | GET  | /posts/:id(.:format) | posts#show |
{:.small-table}

The `PostsController#show` action would receive the `params[:id]` containing "2-my-little-chthulu".
{:.fragment}

The controller finds the post in the `set_post` before action callback and loads the post with `id` equal to 2.
{:.fragment}
