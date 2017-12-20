Arboreal - Henrik Andersson Qvarfordt

Utgångspunkten när jag startade denna uppgift var att lära mig mer om flexbox. I och med att sidan inte skulle innhålla så mycket innehåll
tyckte jag att det var passande att göra en single-page lösning.
Började med att lägga upp olikfärgade "boxar"  för att se hur de interagerade med varandra. När jag var nöjd började jag med att styla sidan.
Den absolut största tiden har jag lagt på flexbox så "designen" fick inte lika hög prioritet, vilket kanske syns.
Hittade en färgkarta på nätet (http://bit.ly/2ADeQ7E) som jag utgick ifrån. Det var svårt att få texten läsbar mot de olika färgerna så
beslutade att ha en semi-tranparent vit bakgrund till all text. Tyvärr gör det att sidan blir lite väl "fyrkantig" och "boxig", men läsbarheten tyckte jag
var viktigare och jag fick en bra övning i flexbox.
Fonten hittade jag på Google Fonts. Den är utan serifer vilket även det ökar läsbarheten. 
Tyckte det var viktigt att från början försöka få sidan att passa i en mindre skärm, så alla element är stylade med relativa enheter som vh, vw, em osv.
Det är inte perfekt ännu men det fungerar delvis. Lyckades få texten att skala också med hjälp av calc(px + vw) men jag vet inte riktigt om det 
är "best practice".
Lade till kommentarer till min CSS som närmare förklarar de olika delarna.

Validerade HTML och CSS och fick inga fel.


"Document checking completed. No errors or warnings to show."


"W3C CSS-valideringsresultat för style.css (CSS nivå 3)

Gratulerar! Inga fel har hittats"

Feedback från Victoria.
  
Feedback: 

Du borde främst använda dig av relativa måttenheter: % och rem/em istället px-värden. Här finns en bra länk: 
https://www.w3schools.com/tags/ref_pxtoemconversion.asp 
Använder mig främst av relativa måttenheter. Enda gången px används är för att styra fontstorlek men då används den tillsammans med vw i calc(px + vw) för att styra storlek på font när skärmstorlek ändras.

Det skulle vara bra om du lade till rubrikerna Home och About i själva menyn så man kan länka till de rubrikerna på sidan.
Har valt att inte göra det då menyn inte följer med när man skrollar på sidan, alltså behövs inte Home. About tycker jag är typ samma som Home, dvs ”förstasidan”.

Det skulle vara bra att ha rubriker på de olika delarna av sidan som menyn leder till.T.ex. About, Themes, Pricing och Contact. Namn på de olika rubrikerna kan läggas in i taggar av typen <h2>.
Detta höll jag med om och har fixat! 

Det saknas namn på företaget. Man kan lägga in namnet i <header> med en tagg av typen <h1>. 
Det var ett medvetet val. Företagsnamnet nämns 3 gånger över ”hero-bilden” på förstasidan vilket jag tycker räcker gott och väl.

Slogan borde flyttas från <footer> till innehåller under rubriken About istället. Du bör inte använda <h1> till slogan. Som alternativ kan du istället använda <p> tillsammans med <strong> eller endast <h3>. 
Gillar att slogan ligger längst ner i footern. Kändes onödigt att upprepa företagets adress där eller skriva någon konstig copyright-text. Bytte dock till h3.

Information om företaget kan man lägga in i en <p> tag istället för <h2>. <h2> passar jättebra för namn på de olika rubrikerna. 
Fixat!

Det skulle passa bäst om du använder <li> till tabellen med priser istället för <p> taggar. 
Fixat!

Det ska vara bra om du använder <button> för knappar istället för <p> taggar i Pris rubriken. 
Fixat!

Inputfälten <input type="submit">  i rubriken Contact saknar value="Submit". 
Fixat!

Priset för alternativet längst till höger är ojämnt jämfört de andra två alternativen. Det skulle se bättre ut om dessa låg på samma rad. 
Detta kunde jag för mitt liv inte fixa. Så det får ligga kvar som det är.

Det är bättre att lägga rubriker som About,Themes och Pricing i <section> och  deras små underrubriker i <article> istället. 
Förstår! Men jag följde exemplet högts upp på denna sida: https://www.w3schools.com/tags/tag_section.asp. Så jag tror att det går att använda <section> på det sättet som jag gjort.

Det är bättre att lägga in contact information(adressen,mail, sitemap,twitter och facebook) i <footer> istället. Här finns en bra länk https://www.w3schools.com/tags/tag_footer.asp 
Jag valde att lägga kontaktinfo bredvid kontaktformuläret istället och ville inte upprepa samma info igen i footer. 

Det finns upprepande av egenskaper i CSS: color: #49654C; Det går att använda sig av variabler för att återanvända kod i CSS: 
https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables 
Känner till det, men i det här fallet används bara 4 färger. Så tyckte inte det var nödvändigt.

Använd större marginaler mellan de olika rubrikerna 
Använd större padding för att göra känslan av sidan luftigare  
Har ökat padding och margin något.
