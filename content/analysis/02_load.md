---
Title: Load
Description: Load analysis
Template: index
---

Utvärdera webbplatsers laddningstid och användbarhet
=======================

Uppgiften går ut på att välja ett antal olika webbplatser (minst 3), testa deras laddningstid och ge förslag på hur de kan gå till väga för att förbättra laddningstiden samt även användbarheten av sidan.

Urval
-----------------------

Jag valde https://unsplash.com/, https://www.pexels.com/ och https://pixabay.com/ för de är sidor med många bilder som kan påverka en sidas laddningstider drastiskt. Dessa är de sidor som rekommenderades till oss som resurser för att hämta ut rättighetsfria bilder.

Metod
-----------------------

Jag kommer att använda mig av både Chromes inbyggda nätverks verktyg samt Google Pagespeed för att mäta webbsidornas laddningstid. Jag kommer att mäta hur snabbt webbsidorna laddas både på desktop och mobile. De kommer göras 3 mätningar per sida som sedan sammanställs till ett medelvärde. Jag kommer undersöka; startsidan, en resurs-sida samt inloggningssidan. Om de använder sig av en inloggnings-modal kommer jag istället ta en annan resurssnål sida. De värden som observeras kommer sedan läggas i en tabell och visas upp i rapporten.

Resultat
-----------------------

### Unsplash

Unsplash hade en relativt snabb webbplats. Startsidan hade laddningstider under 500 ms och fick ett Google Pagespeed resultat på 55 poäng (mobil) samt 76 poäng (desktop). Resurssidan laddade nästan lika snabbt som startsidan som är ett bra tecken på att de har haft prestanda i åtanke när de har gjort webbplatsen. Inloggningssidan var dock ganska långsam given de få resurser som behövdes laddas in. Den var den långsammaste av de tre webbsidorna med 30% längre laddningstid än startsidan. Dock gav Google Pagespeed webbsidan 65 poäng (mobil) och 98 poäng (desktop), de högsta poängen av webbsidorna. Detta var inte vad jag hade förväntat mig. Inloggningssidorna på webbplatser brukar ha de lägsta laddningstiderna vilket kan betyda att resultatet kan ha påverkats av andra faktorer t.ex. Webbläsarens addons.

<img src="../image/kmom05/Unsplash.png?w=100%">

### Pexels

Pexels var i stora överlag den minst optimerade webbplatsen. Alla webbsidor på webbplatsen hade höga storlekar på sidorna med många resurser som behövde laddas. Resurssidan laddade 150 megabyte av resurser, mer än 100 gånger så många resurser som de andra webbplatserna. Detta hände för att de laddade alla bilder på sidan så fort webbsidan laddades, vilket påverkade webbsidans responsivitet väldigt mycket. Om de implementerade antingen mindre bilder i webbsidans design eller laddade mer bilder under tiden man scrollade ner på webbsidan skulle prestandan på sidan öka samt laddningstiderna skulle gå ner. Denna resurssida hade laddningstider mot 2 sekunder, det var den enda sidan som inte laddades under 1 sekund. Startsidan var i relation till de andra webbplatserna även den långsam. Den hade den sämsta laddningstiden av de 3 startsidorna samt även det sämsta Google Pagespeed poängen. Inloggningssidan var också den väldigt långsam då sidan laddade in ett tio-par bilder som den använde som bakgrund.

<img src="../image/kmom05/Pexels.png?w=100%">

### Pixabay

Pixabay var den mest optimerade av de 3 sidorna. Den hade en ganska snabb hemsida, ungefär lika snabb som Unsplash med laddningstider runt 500ms eller lägre. Dess Google Pagespeed resultat var väldigt bra på desktop med ett medelvärde på 83 poäng. Dock hade den ett lägre mobilt resultat med endast 46 poäng. Resurssidan var även den väldigt snabb med ungefär samma laddningstider som hemsidan. Där fick den igen ett väldigt bra desktop resultat (90 poäng) men återigen ett sämre mobilt resultat (47 poäng). Deras största problem när det kommer till optimering verkar vara deras mobila design. De hade ingen inloggningssida utan använde sig utav en inloggningsruta istället. Därför valde jag att undersöka deras om-sida istället. Den hade liknande laddningstider som de andra webbplatsernas inloggningssida, fast använde sig utav mer resurser.

<img src="../image/kmom05/Pixabay.png?w=100%">

Analys
-----------------------

Jag fann att Pixabay var den snabbaste webbsidan. Den hade bäst Google Pagespeed resultat på desktop och skapliga resultat på mobil. Pixabay använde sig mycket av lazy-loading, vilket betyder att de laddade in mer resurser ju längre ner på sidan man kom vilket drastiskt förminskade de initiala laddningstiderna. Unsplash var nästa bäst då de använde en liknande design som Pixabay medan Pexels valde att ladda massor av resurser på en gång, vilket gav dem väldigt långa laddningstider. Pixabay använde sig även av mycket mindre bilder än vad Unsplash och Pexels gjorde. Detta sänkte mängden data som behövdes laddas in utan att egentligen förstöra webbsidans utseende. Både Unsplash och Pexels använde sig utav 600 pixlar breda bilder medan Pixabay använde sig av hälften så stora bilder, 300 pixlar.

De största åtgärden som dessa webbplatser använde sig utav var lazy-load och mindre bildstorlekar. Man kan även förbättra laddningstiderna på andra sätt, t.ex. Att ändra designen på webbsidorna och visa mindre bilder. Dock kan detta vara svårt för dessa typer av webbsidor som visar upp otroligt många bilder.

### Rangordning

1. Pixabay
2. Unsplash
3. Pexels

Pixabay var den snabbaste samt även den som fokuserade mest på optimering av de 3 sidorna. Unsplash var en nära tvåa medan Pexels inte gjorde väldigt mycket för att optimera sin sida.

### Laddningstids gräns

Jag upplevde inte någon större degradering av användbarheten på dessa sidor dock skulle jag kunna tänka mig att någon på, t.ex. En mobil skulle ha en sämre upplevelse på dessa sidor. Den lägsta gränsen jag kan tänkas tolerera när det kommer till laddningstider skulle vara runt 3-5 sekunder. Över detta blir det väldigt svårt att använda en webbplats, speciellt om den använder sig av många sidbyten. Alla 3 webbplatser var under denna gräns, dock så gav Pexels en sämre upplevelse.

Referenser
-----------------------

### Rådata

<iframe style="width:100%; height: 100vh;"src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTuQzNZZFLKsnBzI3r0AKZbTis1TkjWDIu-fPr1NWw4_dDcsgZosKk68oj67itg_nkvIs-WpaeJzbbY/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false"></iframe>

Övrigt
-----------------------

Anton Torrijos Bergman