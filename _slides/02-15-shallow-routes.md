---
layout: slide
---

## Resulting Shallow Routes

|          Prefix | Verb   | URI Pattern                            | Controller#Action |
|----------------:|:-------|:---------------------------------------|:------------------|
|   post_comments | GET    | /posts/:post_id/comments(.:format)     | comments#index    |
|                 | POST   | /posts/:post_id/comments(.:format)     | comments#create   |
|new_post_comment | GET    | /posts/:post_id/comments/new(.:format) | comments#new      |
|    edit_comment | GET    | /comments/:id/edit(.:format)           | comments#edit     |
|         comment | GET    | /comments/:id(.:format)                | comments#show     |
|                 | PATCH  | /comments/:id(.:format)                | comments#update   |
|                 | PUT    | /comments/:id(.:format)                | comments#update   |
|                 | DELETE | /comments/:id(.:format)                | comments#destroy  |
{:.small-table}
