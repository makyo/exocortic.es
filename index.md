---
layout: default
---

> A century or two before [*Post-Self*](http://post-self.io), before the advent of uploading, humanity had just begun to dabble in exocortices and managed sensoria. They offloaded some of the work the brain was performing onto other substrates --- bubble memories, organic processors...hardware instead of wetware.
>
> As in all late capitalist economies, with every scientific advance came a whole host of products.
>
> Some good, some bad.
>
>Some useful, some fun, mere toys.
>
> And this is when humanity started changing.

-----

There is a description of [the universe](/about/universe) in which the stories take place and some [shared characters](/about/characters) which authors may use, and the [existing entries](/entries) posted from the creators involved in the project upon which to build.
{: class="excerpt offset" }

{% if site.categories.entry.size > 0 %}
<div class="entries">
    <h2>Most recent</h2>
    {% for post in site.categories.entry limit: 3 %}
        {% include entry.html post=post %}
    {% endfor %}
    {% if site.categories.entry.size > 3 %}
        <p class="to-entries"><a href="/entries">More entries</a></p>
    {% endif %}
</div>
{% endif %}

{% if site.categories.news.size > 0 %}
<div class="news">
    <h2>News</h2>
    {% for post in site.categories.news limit: 3 %}
        {% include entry.html post=post %}
    {% endfor %}
    {% if site.categories.news.size > 3 %}
        <p class="to-entries"><a href="/entries">More entries</a></p>
    {% endif %}
</div>
{% endif %}

Have an idea for a story? A change you'd like to see on the site? Check out the [contributing guidelines](/about/contributing) and create a pull-request or file an issue.
