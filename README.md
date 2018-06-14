## Custom div Class Markdown Extension

Forked from [exaroth/mdx_custom_span_class](https://github.com/exaroth/mdx_custom_span_class)

This is a simple extension for Python-Markdown library, which allows adding div elements with custom class.
The syntax is:
```
!!<class name>|<text to be wrapped>!!
```
For instance:

```shell
I love !!text-alert|spam!!
```
will return

```html
<p>I love <div class="text-alert">spam</div></p>
```


### Installation

```shell
pip install git+git://github.com/Anders-Linden/mdx_custom_div_class.git
```

### Usage

```python
import markdown

md = markdown.Markdown(extensions=["custom_div_class"])
md.convert("I love !!text-danger|spam!!")

```

