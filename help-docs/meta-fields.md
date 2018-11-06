# Meta Fields

You can add Meta Fields to your content types

### How to add

You can add Meta Fields within the content type:

![alt text](https://github.com/clixell/clixell-content/blob/master/help-docs/images/how-to-meta-1.jpg)

Call the Meta fields with the following code:

```
meta title: {{ content_meta_title }}
meta desc: {{ content_meta_desc }}
{% assign custom_meta_title = content_meta_title %}
{% assign custom_meta_desc = content_meta_title %}
```
