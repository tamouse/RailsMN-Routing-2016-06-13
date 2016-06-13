---
layout: slide
---

### Note:

Because the router uses the HTTP verb **and** the URL to match the route,
four URLs can map to seven different actions.

| URL | Verb |
|:----|:-----|
| /posts | GET (index), POST (create) |
| /posts/:id | GET (read), PUT (update), DELETE (destroy)|
| /posts/:id/new | GET (new) |
| /posts/:id/edit | GET (edit) |
{: .small-table .fragment}
