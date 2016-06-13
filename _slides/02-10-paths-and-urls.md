---
layout: slide
---

## Path and URL Helpers

The third thing that Rails routing does is provide **helper** methods for the paths and URLs associated with a given controller and action.

<small><em>assume <code>@post.id == 10</code></em></small>

| Helper Method | Result |
|:--------------|:-------|
| <code>posts_path</code> | <code>/posts</code> |
| <code>posts_url</code> | <code>https://example.com/posts</code> |
| <code>edit_posts_path(@post)</code> | <code>/posts/10/edit</code> |
| <code>edit_posts_url(@post)</code> | <code>https://example.com/posts/10/edit</code> |
{:.small-table}
