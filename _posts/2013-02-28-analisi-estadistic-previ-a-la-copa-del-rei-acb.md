---
layout: post
title: Anàlisi estadístic previ a la Copa del Rei ACB
date: 2013-02-28 19:39
comments: true
categories: [pro]
---
<img alt="Copa del Rey 2012" src="http://farm8.staticflickr.com/7053/6912046471_ea24557470_z.jpg" width="640" height="396" />

La Copa del Rei ACB, és una de les competicions esportives més emocionants. Els vuit millors equips al final de la primera volta de la lliga disputen el títol. Durant quatre dies, en una sola seu, i amb un sistema de competició que no accepta la derrota. Aquest esdeveniment és la gran festa del bàsquet.

### Punt de partida

Sorprès pel poc favoritisme del FC Barcelona (FCB) abans de disputar-se l'edició del 2013, vaig preguntar-me si la posició a la lliga en què es classifiquen els equips (el FCB va ser el 7è classificat) té relació amb la posició final a la Copa.

### Metodologia


* Assigno el valor posició final copa, en funció del darrer partit jugat (**1 = campió, 2 = finalista, 3 = semifinals, 4 = quarts de final**).
* L'estudi inicial contemplava les darreres 10 edicions. Una vegada escrit el codi, he ampliat l'estudi amb l'edició del 2013.
* Pels gràfics de punts rebuts i punts anotats s'adjudica un valor (de l'1 al 8) en funció de la posició de cada equip en cada classificació. Es perd exactitud, però facilita el càlcul.
* No es té en compte l'equip amfitrió de cada edició. Aquest equip és convidat a disputar la Copa sense importar la seva classificació al final del a primera volta. Sempre estudiem els 8 primers classificats.
* Dades de la pàgina oficial de l'ACB (<a title="ACB" href="http://www.acb.com">www.acb.com</a>).
* Càlculs i gràfics possibles gràcies a R <a title="R-Project" href="http://www.r-project.org/">(www.r-project.org)</a>.


### Posició a la lliga

A priori, la posició a la lliga en què cada equip es classifica per a la Copa del Rei és rellevant en la posició final. Com podem observar en el gràfic següent, l'afirmació té un cert sentit.

De les 11 anys edicions estudiades, en 5  (del 2008 fins a 2012) hi ha una clara relació entre posició a la lliga i posició a la copa.

És una relació lògica, ja que la posició a la lliga en què es classifica cada equip, ve donada pel nombre de victories els primers mesos de competició.

Casualment aquest any 2013, la tendència de les darreres 5 edicions canvia. Apuntar que el primer classificat a la lliga va caure derrotat pel que seria campió de la competició.

<a title="ACB - Copa del rei 2003 - 2013 [Posició final vs Posició lliga] by Sergi Xaudiera, on Flickr" href="http://www.flickr.com/photos/sergixaudiera/8491825009/"><img alt="ACB - Copa del rei 2003 - 2013 [Posició final vs Posició lliga]" src="http://farm9.staticflickr.com/8231/8491825009_ab25dec1cf_z.jpg" width="640" height="455" /></a>

###Punts a favor

Els punts a favor d'un equip indiquen la facilitat que té aquest per anotar. Observem poca relació  entre punts anotats i posició final de cada equip a la Copa.

Les edicions  de 2008 i 2010 són les que hi ha una relació més pronunciada entre punts anotats i posició final a la lliga.

Comparant el gràfic amb l'anterior de posició a la lliga, la relació entre variables és bastant inferior.

Pel que fa el FCB, només en l'edició de 2010 es classifica com l'equip màxim anotador i acaba coronat campió.

<a title="ACB - Copa del rei 2003 - 2013 [Posició final vs Punts a favors] by Sergi Xaudiera, on Flickr" href="http://www.flickr.com/photos/sergixaudiera/8491824953/"><img alt="ACB - Copa del rei 2003 - 2013 [Posició final vs Punts a favors]" src="http://farm9.staticflickr.com/8509/8491824953_9741ac9257_z.jpg" width="640" height="455" /></a>

### Punts en contra

Els punts en contra d'un equip indiquen la dificultat que tenen els seus rivals per anotar punts quan s'hi enfronten. A un primer cop d'ull no s'observa, fins el 2007,  relació entre punts en contra i la posició final a la Copa.

Entrant al detall, veiem com la relació entre punts rebuts i posició final a la Copa, és especialment destacada a partir de 2009.

L'edició de 2009 és especialment significativa. Els 4 primers classificats a la copa coincideixen amb els 4 equips que menys punts havien rebut a final de la primera volta.

En les darreres 4 edicions el FCB és l'equip amb menys punts en contra dels que disputen la copa. En totes les ocasions a arriba a disputar la final del torneig, i en 3 ocasions la guanya.

<a title="ACB - Copa del rei 2003 - 2013 [Posició final vs Punts en contra] by Sergi Xaudiera, on Flickr" href="http://www.flickr.com/photos/sergixaudiera/8491824979/"><img alt="ACB - Copa del rei 2003 - 2013 [Posició final vs Punts en contra]" src="http://farm9.staticflickr.com/8376/8491824979_48a9838101_z.jpg" width="640" height="455" /></a>

### Conclusió

Les opcions que té un equip de guanyar la Copa del Rei ACB no estan només relacionades amb la posició a la lliga en què es classifica.

Els punts en contra és un indicador tant o més vàlid que la posició a la lliga en què s'ha classificat, i té un alt grau de relació amb la posició final a la Copa, especialment en el cas del FCB. Si l'equip blaugrana es classifica a la Copa amb la millor defensa la probabilitat de ser-ne el campió és molt alta.

Per altre banda, els punts a favor no resulten tan determinants per preveure la posició final de cada equip.
