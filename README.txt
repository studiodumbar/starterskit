*********************************************************

+++++            Starters Kit - HTML/CSS            +++++

*********************************************************

Om een overzicht te verkrijgen van alle pagina's die deel uitmaken van de Starters Kit, open de 'index.html' pagina in een (van de onderstaande) webbrowsers.

Voor het 'Webrichtlijneninspectie' rapport (en ook alle andere vragen omtrent de Starters Kit) kan men terecht bij project 1 Logo (1logo@minaz.nl).

*********************************************************

De Starters Kit is uitgebreid getest in de volgende browsers:

Windows
- IE6
- IE7
- IE8
- Safari 4
- Firefox 3 en 3.5
- Opera 10
- Chrome 2b

Mac
- Safari 4
- Firefox 3.5
- Opera 10


*********************************************************
++++++++++++++++++++++   VERSIES   ++++++++++++++++++++++
*********************************************************

versie 	1.2.3
datum	13 april 2010

=> De 16 basiskleuren en bijbehorende afgeleide lichtere en lichtste kleuren voor digitale middelen (internet) zijn begin 2010 gewijzigd.
=> De nieuwe kleuren zijn in deze versie van de Starterskit doorgevoerd. De 'oude' kleuren zijn vervangen door de nieuwe kleuren.

=> stylesheets gewijzigd
1) color.css
2) forms.css (minimaal; enkel kleur gerelateerd)
3) screen.css (minimaal; enkel kleur gerelateerd)

*********************************************************

versie 	1.2.2
datum	30 november 2009

=> De 'tong' begint nu precies in het midden (dit geld niet voor IE6/7!)
=> Opgelost ontbreken van witte pijltje in arrows.png (voor witte tekst in tong)
=> Line-height H1 aangepast (regelafstand was te groot)

=> stylesheets gewijzigd
1) screen.css
2) template.css
3) type.css
4) ie/ie7.css

=> plaatjes gewijzigd
1) css/skin/arrows.png

*********************************************************

versie 	1.2.1
datum	20 november 2009

=> Hoofdnavigatie ('nav_main') was nog Verdana i.p.v. Arial

=> stylesheets gewijzigd
1) screen.css
2) type.css

*********************************************************

versie 	1.2.
datum	3 november 2009

=> bevindingen webrichtlijnen inspectie doorgevoerd
=> pagina's zie (minimaal) gewijzigd zijn:

1) basis_elementen.html
2) content_6.html
3) home_5.html
4) content_3.html
5) content_4.html

=> stylesheets zijn (wederom) minimaal gewijzigd
1) type.css
2) forms.css
3) ie/ie6.css
4) ie/ie7.css

*********************************************************

versie 	1.1
datum	15 oktober 2009

=> pagina's toegevoegd zijn:

1) content_7.html		(lijstpagina)
2) content_8.html		(functionele links, toolbox)
3) zoekresultaten_1.html	(zoekresultaten)
4) zoekresultaten_2.html	(zoekresultaten, breed)
5) sitemap.html			(sitemap)

*********************************************************

versie 	1.0
datum	10 september 2009

=> eerste versie!


*********************************************************
++++++++++++++++++++   OPMERKINGEN   ++++++++++++++++++++
*********************************************************

Er is een klein verschil in het renderen van fonts tussen Firefox (3 en 3.5) op een Mac en een PC.
=> Dit is enkel en alleen 'storend' en zichtbaar in de algemene zoek rechts bovenaan in de header.
=> De hoogte van de zoek button (input.submit) is iets hoger dan het invoerveld (input.text).
=> Dit wordt geregeld in de forms.css stylesheet ( .search form input.text, x:-moz-any-link { padding-bottom: 0.1em; } ).
=> Het is nu zo 'ingesteld' dat het correct (input.submit en input.text even hoog) is in Firefox op een PC.
=> Verwijder de gehele Firefox specifieke regel of verander de padding-bottom in 0.2em en het is correct in Firefox op de Mac.
=> Elke tip om dit voor zowel de Mac als PC versie correct te krijgen is uiteraard welkom!

*********************************************************

De Starters Kit is getoetst op webrichtlijnen, alle bevindingen zijn verwerkt op de volgende punten na (achter de pijlen => staat reactie Studio Dumbar waarom niet):

1) "CSS validatie geeft fouten. ie6.css ie7.css"
=> Dit is (helaas) noodzakelijk, omdat IE6/7 niet webstandards compliant browsers zijn.
=> Om er voor te zorgen dat de Starters Kit pagina's er min of meer hetzelfde uitzien als in de moderne webstandards compliant browsers (zoals Firefox, Safari, Opera, etc.), worder er aan een aantal IE specifieke stijlen en/of exploits aan IE voorgeschoteld.
=> Een property zoals 'zoom' valideert inderdaad niet, want niet webstandaard, maar Microsoft 'proprietary', maar lost wel een aantal 'has Layout' problemen op.

2) "CSS validatie geeft fouten. forms.css"
=> Na een Google zoek aktie het volgende gevonden betreffende 'floated elements need to have a width declared', namelijk: "... On the other hand, the checker will sometimes issue 'warnings' such as the ones you described above even if the document has no errors."
=> http://www.highdots.com/forums/cascading-style-sheets/re-applying-width-floated-elements-272606.html
=> En de W3C zegt het volgende over floated elementen zonder breedte gedefinieerd: "If 'width' is computed as 'auto', the used value is the "shrink-to-fit" width."
=> http://www.w3.org/TR/CSS21/visudet.html#float-width

3) "De (sub)navigatie menu moet onderaan"
=> Op de webrichtlijnen website (http://webrichtlijnen.nl/handleiding/ontwikkeling/productie/paginastructuur/body/#r-pd-6-2) staat er bij Volgorde van belangrijkheid dat de inhoud van een pagina is het aan te raden om deze in volgorde van belangrijkheid in de HTML te zetten.
=> Daarnaast wordt er ook verwezen naar het overslaan van lange navigatielijsten (http://webrichtlijnen.nl/handleiding/ontwikkeling/productie/links-navigatie/seriele-navigatie/#lange-lijsten-overslaan).
=> Op de Fronteers website is ook een hele discussie (http://fronteers.nl/blog/2008/05/webrichtlijnen-volgorde-van-belangrijkheid) over deze volgorde van belangrijkheid met verschillende meningen en uitkomsten, dus niet eenduidig.
=> In het geval van de Starters Kit, is de hoofdnavigatie (daar gaat het hier om) niet heel erg lang (tussen de 3 en 7 links). Het visueel ontwerp (shaduwrand plus schaalbaarheid) maakte het onmogelijk om de hoofdnavigatie onderaan de pagina te plaatsen in de HTML, daarentegen staat de subnavigatie wel onderaan de pagina en worden er skip en jump links aangeboden.

*********************************************************