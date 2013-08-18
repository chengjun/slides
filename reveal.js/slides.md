% Title
% Name
% Date


About
---

### Cheng-Jun Wang
#### 2013/8/18 19:58:33 
![](http://s3.amazonaws.com/hakim-static/portfolio/images/rvl-js.jpg)


My first slide
--------------------

List

* this 
* is
* cool

Variables
---------

The following variables can be defined from the command line:

* theme
* transition

```bash
pandoc -t html5 --template=template-revealjs.html \
	--standalone --section-divs \
  --variable theme="beige" \
  --variable transition="linear" \
  slides.md -o slides.html
```