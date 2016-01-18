---
layout: post
title:  "Jekyll! Jekyll is all you need!"
date:   2016-01-18 -0800
comments: true
---

In den letzten Jahren merkt man immer mehr den Trend weg von schwergewichtigen DB-based Homepages hin zu leichtgewichtigen Exemplaren.

Die Einstiegshürde für aufstrebende Neublogger war früher wesentlich höher als es heutzutage der Fall ist. Wordpress und andere Mitstreiter erleichtern einem immens das Setup und den Betrieb. Eigentlich beschränkt sich das Setup bei den Blog-Service-Anbietern auf 1. Namen wählen 2. Template aussuchen 3. loslegen.

Als Entwickler bin ich diesen Anbietern bis heute nicht wirklich zugeneigt. Ich argumentierte immer nach der Premisse "Gibt's nicht? Dann programmiere ich es eben selbst!" und hegte so eine gewisse Abneigung gegenüber diesen "Ich klick mir alles zusammen"-Derivaten.

Dank statische Seitengenerator gibt es glücklicherweiße für den DIY-Nerd nun schicke Kits mit denen er mit Markdown-Hacks und herrlichen cmd Befehlen sich seine eigene Homepage zusammen tippen kann.

### Was ihr braucht

Ganz ohne Tools kommt ihr natürlich nicht aus. Beim Erstellen unserer Homepage hilft uns [Jekyll].

Die Basis hinter Jekyll ist ein in Ruby geschriebener Renderer welcher Liquid-like Templates verwendet um daraus sofort deploybare statische Websites generiert. Durch den Support von Jekyll auf Github-Pages gestaltet sich der Akt des Deployments auf eine geeignete Infrastruktur mehr als einfach.

Falls Ihr noch kein Ruby installiert habt findet ihr den Installer auf [Rubylang.org][Ruby]

Um Jekyll zu installieren benutzen man den praktischen Ruby Package Manager [RubyGems]
{% highlight bat linenos %}
gem install jekyll

Fetching: jekyll-3.0.1.gem (100%)
Successfully installed jekyll-3.0.1
Parsing documentation for jekyll-3.0.1
Installing ri documentation for jekyll-3.0.1
Done installing documentation for jekyll after 1 seconds
1 gem installed
{% endhighlight %}

Durch ein eingebautes Boilerplate-Template könnt ihr mit folgenden Befehlen euren ersten Prototypen zum Laufen bekommen:
{% highlight bat linenos %}
jekyll new
New jekyll site installed in C:/mkellenbenz/Code/protojekyll.
{% endhighlight %}

Mit einem Blick ins Verzeichnis findet man nun die erstellte Boilerplate. Diese kann mit folgendem Befehl gebaut und für den lokalen Zugriff bereit gestellt werden.
{% highlight bat linenos %}

jekyll serve

Configuration file: C:/xeTic/Code/testjekyll/_config.yml
       Source: C:/xeTic/Code/testjekyll
       Destination: C:/xeTic/Code/testjekyll/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
                    done in 0.359 seconds.
 Auto-regeneration: enabled for 'C:/xeTic/Code/testjekyll'
Configuration file: C:/xeTic/Code/testjekyll/_config.yml
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
{% endhighlight %}

Das ist nun eure Basis für all eure kreativen Ideen. Wer eine Abkürzung nehmen will kann ich die Seite [JekyllThemes] empfehlen. Sie enthält eine Vielzahl an vorgfertigten Themes wo sicher jeder "sein" Theme finden wird.

Dazu muss aber gesagt sein das eine gehörige Portion Frustrationstolleranz vorhanden sein sollte, da einige Themes auf alten Versionen von Ruby und anderen Gems basieren und sich dadurch das Einrichten der Themes manchmal schwierig gestaltet.

### Fazit

Jekyll bietet euch eine leichtgewichtige und geradlinige Möglichkeit eure eigene Homepage zu erstellen. Wie mit allem gibt es natürlich Vor- und Nachteile, aber die Kombination mit den Deployment-Möglichkeiten macht es zu einem tollen Framework.


[Jekyll]:             https://jekyllrb.com/
[RubyGems]:           https://rubygems.org/pages/download
[Liquid]:             https://github.com/Shopify/liquid/wiki
[Ruby]:               https://rubylang.org
[JekyllThemes]:        http://jekyllthemes.org
