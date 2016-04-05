---
layout: default
title: Papers
---


# Academic Papers

1. [The Cosmic Question](pending)
2. [A Defense of Hylomorphism](pending)
3. [Imaginative Norms: Virtue Ethics and Imagination](pending)

{% for paper in site.papers %}
<h4 class="paper"><a class="post-link" href="{{ paper.url | prepend: site.baseurl }}">{{ paper.title }}</a></h4>
<div class="tagline">{{ paper.tagline | markdownify }}</div>
<div class="source">Source: 
    Source: 
    <a class="source-link" href="{{ paper.path | remove: 'C:/Users/Dan/Dropbox/dansheffler/' | prepend: 'https://raw.githubusercontent.com/dansheffler/dansheffler.com/master/' }}">
        md
    </a>

    | Paper version: 
    <a class="pdf-link" href="{{ paper.path | remove: 'C:/Users/Dan/Dropbox/dansheffler/_papers/' | prepend: '/pdfs/' | remove: '.md' | append: '.pdf' }}">
        pdf
    </a>
    | Permalink: 
    <a class="permalink" href="{{ paper.url | prepend: site.baseurl }}">
        html
    </a>
</div>
{% endfor %}