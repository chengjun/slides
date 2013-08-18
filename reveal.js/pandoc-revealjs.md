% Making Reveal.js Slides with Markdown and Pandoc
% Cheng-Jun Wang
% 2013/8/18 20:31:20 


About REVEAL.JS
---

A framework for easily creating beautiful presentations using HTML. Check out the live demo. Check [here](https://github.com/chengjun/slides/tree/gh-pages/reveal.js).

reveal.js comes with a broad range of features including nested slides, markdown contents, PDF export, speaker notes and a JavaScript API. It's best viewed in a browser with support for CSS 3D transforms but fallbacks are available to make sure your presentation can still be viewed elsewhere.

![](http://s3.amazonaws.com/hakim-static/portfolio/images/rvl-js.jpg)


Install Pandoc
---
![](http://2.bp.blogspot.com/-pxBFVXfcaDk/UfI7gsOaAPI/AAAAAAAAFZQ/TkyEB5b49uE/s200/pandoc+conversion+documentos+doc+rtf+tex+odt+html+wikimedia.PNG)

![](http://www.reactiongifs.com/wp-content/uploads/2012/11/emma-yeah-ok.gif)

Method 1
--------------------

First, Dowload reveal.js from [https://github.com/chengjun/slides/tree/gh-pages/reveal.js](https://github.com/chengjun/slides/tree/gh-pages/reveal.js "https://github.com/chengjun/slides/tree/gh-pages/reveal.js"), uninstall it into one directory.

Second, create a reveal.js template in the reveal.js directory. 

     Edit the demo file index.html in the reveal.js repository. 
     Remove everything inside the <div id="slides">.
     and replace it with $body$. Save this as template.revealjs.

Third, Using powershell, cd into the reveal.js directory.

Fourth, run the pandoc script:

	pandoc --section-divs -t html5 -s \
		   --template template.revealjs \
		   -o myslides.html myslides.txt



Method 2
--------------------

Refer to this link [https://gist.github.com/aaronwolen/5017084](https://gist.github.com/aaronwolen/5017084 "https://gist.github.com/aaronwolen/5017084")

1.Install pandoc, download and uninstall reveal.js 
2.similar to method 1, you need the template-revealjs.html from the above link
3.Using powershell to run pandoc:


	pandoc -t html5 --template=template-revealjs.html \
	    --standalone --section-divs \
	  --variable theme="beige" \
	  --variable transition="linear" \
	  slides.md -o slides.html


Variables in pandoc script
---------

The following variables can be defined from the command line:

* theme
* transition

Go!
---

![](http://i.imgur.com/H9KCl.gif)