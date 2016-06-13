---
layout: slide
---

## Choosing the Controller

Rails determines which controller it should map to by the following **convention**: convert the resource symbol to a string, run [camelize] on it, concatenate the string "Controller", and then [constantize] that.
{:.left-align}

<pre><code class="ruby">(resource_symbol.to_s.camelize + "Controller").constantize</code></pre>

Thus:
{:.left-align .fragment}

<pre><code class="ruby">resources :posts # => PostsController</code></pre>
{:.fragment}

<pre><code class="ruby">"posts#new" # => PostsController#new</code></pre>
{:.fragment}

[camelize]: http://api.rubyonrails.org/classes/ActiveSupport/Inflector.html#method-i-camelize "camelize method ActiveSupport::Inflector"
[constantize]: http://api.rubyonrails.org/classes/ActiveSupport/Inflector.html#method-i-constantize "constantize method in ActiveSupport::Inflector"
