---
layout: slide
---

## What is an HTTP request?

From the [RFC]:

<pre><code>Request = Request-Line
          *(( general-header | request-header | entity-header ) CRLF)
          CRLF
          [ message-body ]</code></pre>

<pre><code>Request-Line = Method SP Request-URI SP HTTP-Version CRLF</code></pre>
{: .fragment }

<pre><code>GET / 1.1</code></pre>
{: .fragment }


[RFC]: https://www.w3.org/Protocols/rfc2616/rfc2616-sec5.html
