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

Feedback från Victoria:

Uppnådda krav:
1)Sidan använder sig av en fler-kolumns-layout.
2)Du använder dig av semantisk HTML för att strukturera upp ditt innehåll.
3)Du använder dig av _class_ och  <tag>  för att styla din sida.
4)Du använder dig huvudsakligen utav flexbox för att positionerna ditt innehåll.
5)Din sida innehåller ett korrekt formaterat kontaktformulär som ska vara en <form>där man kan fylla i namn, telefonnummer, email, företag och meddelande.
6)CSS-filen är logiskt upplagd och lättläst.
7)Tydlig namngivning av klasser så att man förstår vad det är som stylas.
8)HTML och CSS är korrekt indenterad.
9)HTML och CSS validerade korrekt vid kontroll med W3C HTML Validator/W3CCSS Validator.
  
Feedback:
1)Du borde främst använda dig av relativa måttenheter: % och rem/em iställetpx-värden. Här finns en bra länk:https://www.w3schools.com/tags/ref_pxtoemconversion.asp
2)Det skulle vara bra om du lade till rubrikerna Home och About i själva menyn så mankan länka till de rubrikerna på sidan.
3)Det skulle vara bra att ha rubriker på de olika delarna av sidan som menyn leder till.T.ex. About, Themes, Pricing och Contact. Namn på de olika rubrikerna kanläggas in i taggar av typen <h2>.
4)Det saknas namn på företaget. Man kan lägga in namnet i <header> med en tagg avtypen <h1>.
5)Slogan borde flyttas från <footer> till innehåller under rubriken About istället. Du börinte använda <h1> till slogan. Som alternativ kan du istället använda <p> tillsammansmed <strong> eller endast <h3>.
6)Information om företaget kan man lägga in i en <p> tag istället för <h2>. <h2> passar jättebra för namn på de olika rubrikerna.
7)Det skulle passa bäst om du använder <li> till tabellen med priser istället för <p>taggar.22017-12-11
8)Det ska vara bra om du använder <button> för knappar istället för <p> taggar i Prisrubriken.
9)Inputfälten <input type="submit">  i rubriken Contact saknar value="Submit".
10)Priset för alternativet längst till höger är ojämnt jämfört de andra två alternativen. Detskulle se bättre ut om dessa låg på samma rad.
11) Det är bättre att lägga rubriker som About,Themes och Pricing i <section> och  derassmå underrubriker i <article> istället.
12) Det är bättre att lägga in contact information(adressen,mail, sitemap,twitter ochfacebook) i <footer> istället. Här finns en bra länkhttps://www.w3schools.com/tags/tag_footer.asp
13)Det finns upprepande av egenskaper i CSS: color: #49654C; Det går att använda sig av variabler för att återanvända kod i CSS:https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables
14)Använd större marginaler mellan de olika rubrikerna
15) Använd större padding för att göra känslan av sidan luftigare
