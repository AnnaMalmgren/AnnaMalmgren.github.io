---
layout: post
title: Examination 1 del 2
comments: true
date: 2018-11-18 14.03 +0100
permalink: /:year/:month/:day/:title/
---

## robots.txt
robots.txt är en fil som ger instruktioner till webrobotar som till exempel googlebot. Webrobotar kollar först om filen site.url/robots.txt finns och hur den är konfigruerad för att de ska få reda på vilka filer de får tillgång till. Dock är det viktigt att veta att webrobotar kan ignorera robots.txt.  
Jag har valt att ge fri tillgång för alla webrobotar till mina filer eftersom att jag inte har någon fil jag vill dölja. 
{% highlight ruby %}
User-agent: *
Disallow:
{% endhighlight %}

## humans.txt
humans.txt är en text-fil som är till för att presentera personerna bakom webbplatsen samt kort information om webbplatsen och personer eller företag som man vill rikta särskilda tack till. 
Jag har varken twitter eller någon annan webbplats så därför valde jag att utelämna fakta om det.
{% highlight ruby %}
/* TEAM */
Developer: Anna Malmgren 
From: Lund, Sweden

/* Site */
Last update: 2018/11/19
Language: svenska
IDE: Visual Studio Code
Components: Jekyll, Sass.
{% endhighlight %}  


## Kommentarer
För att lägga till möjligheten att kommentera blogginlägg använde jag mig av Disqus. Jag skapade en disqus.html fil i _includes mappen för att kunna inkludera den i post.html filen. I disqus.html använde jag disqus universal kod och på de sidor som jag vill kunna möjliggöra kommentarer skapar jag en Front Matter variabel `comments: true`.  

## Open Graph
Open Graph används för att kunna presentera webbsidor på sociala medier på ett så bra sätt som möjligt där man specifiserar titel, typ, bild och url med tags. Det finns även möjlighet att lägga till andra tags om man så önskar. Jag har placerat en open-graph.html fil i _includes och inkluderat den i min head.html fil.
För att göra en webbplats till ett open graph objekt så skall man lägga till ett antal meta taggar i head. De meta property som måste finnas med är alltså titel, type, image och url. I html taggen läggs även ett prefix till.
Mitt mål med min open graph är att skapa en tydlig bild av vad min länk leder till och har lagt in ett antal meta taggar för detta. 