Rapport Kmom05
=======================

I denna rapport har jag valt tre webbplatser och tre undersidor till webbplatserna där jag testar hur snabbt sidorna laddas, antal resurser, storlek på sidan och även hur sidan presterar i Googles PageSpeed test. Därefter kommer jag analysera resultatet och bedöma om det finns någon förbättringspotential avseende användarupplevelsen och laddningstiden.

Urval
-----------------------

Jag har i denna rapport valt att analysera Sveriges tre största e-handlare (Ehandel 2018). Jag valde denna typ av hemsidor på grund av att webbplatser av denna typ ofta kan innehålla mycket bilder vilket kan öka laddningstiden på webbplatsen och därmed försämra kundupplevelsen. De sidor som jag kommer analysera är:

- Dustin Home, www.dustinhome.se
- CDON, www.cdon.se
- Adlibris, www.adlibris.se

För att göra en någorlunda rättvis jämförelse mellan webbplatserna så valde jag att jämföra liknande undersidor på varje hemsida. Jag valde följande undersidor:

- Home-sidan (index)
- En produktsida
- Kundtjänstsidan

Metod
-----------------------

För att utföra testerna där jag mäter webbsidans prestanda har jag använt mig av Googles Pagespeed verktyg. Vertyget kördes i Google Chromes DevTools i inkognitofönster och med inställningen "no throttling". Laddningstid, resurser och storlek mäter jag i DevTools nätverksflik, vid hämtning av resultaten gör jag en hård inläsning där jag även tömmer cacheminnet. Varje sida kommer testas tre gånger och varje resultat som presenteras i rapporten är ett genomsnitt av resultaten.

Resultat
-----------------------

[Resultatet från mätningarna](https://docs.google.com/spreadsheets/d/1r6dI-iNUn3oM6nW8i51T_xHEkp0RpbIEx-TEV_tuXH8/edit?folder=0AMRI9eTokDghUk9PVA#gid=0)

######Dustin Home

[FIGURE src="image/dustin.png?w=500" class="right" caption="Dustin Home"]

På samtliga mobilanpassade och datoranpassade undersidor fick Dustin Home 100/100 som betyg i Google Pagespeeds "Performance" index. Laddningstiderna för de datoranpassade sidorna var något högre än för de mobilanpassade. Förstasidan  hade en laddningstid på 2.24 sekunder för den datoranpassade sidan och 2.17 för den mobilanpassade. De åtgärder som Google Pagespeed rekommenderade för att effektivisera sidan som sparade mest tid var att uppdatera bildformaten samt att optimera bilderna. Dessa åtgärder sparar 0.85 sekunder på mobilsidan och 0.79 på den datoranpassade. Utav Dustin Homes tre undersidor var förstasidan den största.

Resultaten på de två resterande undersidorna speglar resultatet från förstasidan. Även här hämtade de datoranpassade sidorna mer resurser, var större och tog längre tid att ladda. Då dessa sidor var mindre i storlek och inte innehöll lika mycket bilder kunde man inte spara lika mycket i laddningstid genom att optimera sidorna som med förstasidan. På produktsidan kunde en optimering av bilder spara 0.53 sekunder.


######CDON

[FIGURE src="image/cdon.png?w=500" class="right" caption="CDON"]

I "Performance"-indexet fick CDONs förstasida ett resultat på 99 för den mobilanpassade sidan och 98 för den datoranpassade. Noterbart är att den datoranpassade sidan hämtar 176 resurser medan den mobilanpassade endast hämtar 60. Skillnaden i storlek mellan vyerna blir därmed 4.2mb. Laddningstiderna för förstasidan är 2.46 sekunder för den datoranpassade och 1.37 sekunder för den mobilanpassade sidan. En av de optimeringsåtgärder som föreslås är att eliminera resursblockerande resurser, vilket i detta fall rör typsnitt och Javascript.

Produktsidan var i detta fallet större än förstasidan och skillnaden mellan den mobilanpassade och den datoranpassade var endast 1.3MB. Skillnaden i laddningstid mellan vyerna blir därmed inte lika stor som i de tidigare fallen utan är endast 0.06 sekunder. Den totala laddningstiden för den datoranpassade sidan var 2.46 sekunder och storleken 8.9MB. Här rekommenderas samma optimeringsåtgärd som på förstasidan.

Kundtjänstsidan var den sida som tog minst resurser och var lika stor i de båda vyerna. Storleken var 1.2MB och den hämtade 24 resurser. Laddningstiden var 0.49 sekunder för den datoranpassade och 0.51 sekunder för den mobilanpassade. Här sparades mest laddningstid genom att ta bort oanvänd CSS-kod.

######Adlibris

[FIGURE src="image/adlibris.png?w=500" class="right" caption="Adlibris"]

Pagespeeds "Performance"-index hamnade på 100 på samtliga undersidor hos Adlibris. Skillnaden i laddningstid mellan den mobilanpassade vyn och den datoranpassade låg endast på ett par tiondels sekunder. Kundtjänstsidan var den största utav dessa tre undersidor och hamnade på 2.7mb med 56 hämtade resurser för den datoranpassade vyn. Laddningstiden på 1.31 sekunder var dock kortare här än vad den var på den något mindre förstasidan. Mindre optimeringar kunde göras genom att bland annat ta bort oanvänd CSS.

Förstasidan var trots att den innehöll mer bilder och 33 fler hämtade resurser än kundtjänstsidan mindre och hamnade på 2.4mb. Laddningstiden var 2.09 sekunder och två optimeringar som föreslogs var att uppdatera bildformat samt optimera bilder.

Inga optimeringar föreslogs för Adlibris produktsida. Laddningstiden låg här på 1.33 sekunder, antal resurser som hämtades var 68.5 och storleken på sidan 1.4mb.

Analys
-----------------------

Att nästan samtliga sidor hade större datoranpassade sidor var ett resultat som jag hade förväntat mig, då jag anade att de flesta sidorna gömmer innehåll i den mobilanpassade vyn och använder sig av mindre bilder, vilket var fallet. Något som överraskade var att både Dustin Home och CDON hade längre laddningstider på produktsidan än på förstasidan. Jag gjorde antagandet innan rapporten att förstasidan skulle innehålla fler bilder i marknadsföringssyfte men i själva verket var det produktsidorna som innehöll fler bilder i form av reklam för liknande produkter eller fler bilder på produkten. Som väntat var kundservice-sidorna de som hämtade minst resurser och tog kortast tid att ladda, troligen på grund av avsaknaden av bilder.

När jag gjorde mätningarna hade alla sidorna hade perfekta resultat i "Performance"-indexet. På grund av att det är e-handelsföretag som jag har gjort undersökningen på så tror jag att detta är något som de har jobbat aktivt med. Ett lägre resultat hade inneburit en lägre ranking i Googles sökalgoritmer (Wang, Z et Phan D 2018) vilket troligen hade inneburit färre potentiella kunder.

Min gräns för hur länge en sida ska ladda tycker jag ligger mellan 2-3 sekunder. Samtliga sidor låg inom denna gräns. Den sidan som jag tycker klarade sig bäst i undersökningen var Adlibris. Laddningstiderna var lägst och låg som genomsnitt över samtliga undersidor på 1.44 sekunder för den datoranpassade och 1.44 för den mobilanpassade. Samtidigt var antalet resurser och storlek på sidan snarlik mellan den mobila vyn och datorvyn. Detta tyder på att Adlibris inte döljer innehåll när man växlar mellan vyerna och har optimerat sina bilder. CDON kommer på en andraplats då trots webbplatsen är större och hämtar fler resurser än Dustin Home så är laddningstiden lägre.

Slutlig ranking:

1. Adlibris
2. CDON
3. Dustin Home

Referenser
-----------------------

Ehandel (2018). Sveriges 100 största e-handlare.  https://www.ehandel.se/Sveriges-100-storsta-e-handlare,11857.html [2019-12-17]

Wang, Z et Phan D (2018). Using Page speed in mobile search rankings.  https://webmasters.googleblog.com/2018/01/using-page-speed-in-mobile-search.html [2019-12-17]

Övrigt
-----------------------

Niko Ollikainen, 2019-12-17
