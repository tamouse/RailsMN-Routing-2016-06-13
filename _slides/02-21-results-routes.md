---
layout: slide
---

### Resulting Namespaced Routes:

|          Prefix | Verb   | URI Pattern                            | Controller#Action  |
|----------------:|:-------|:---------------------------------------|:-------------------|
|     admin_users | GET    | /admin/users(.:format)                 | admin/users#index  |
|                 | POST   | /admin/users(.:format)                 | admin/users#create |
|  new_admin_user | GET    | /admin/users/new(.:format)             | admin/users#new    |
| edit_admin_user | GET    | /admin/users/:id/edit(.:format)        | admin/users#edit   |
|      admin_user | GET    | /admin/users/:id(.:format)             | admin/users#show   |
|                 | PUT    | /admin/users/:id(.:format)             | admin/users#update |
|                 | DELETE | /admin/users/:id(.:format)             | admin/users#destroy|
{:.small-table}
