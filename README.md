Arboreal - Henrik Andersson Qvarfordt

Utg�ngspunkten n�r jag startade denna uppgift var att l�ra mig mer om flexbox. I och med att sidan inte skulle innh�lla s� mycket inneh�ll
tyckte jag att det var passande att g�ra en single-page l�sning.
B�rjade med att l�gga upp olikf�rgade "boxar"  f�r att se hur de interagerade med varandra. N�r jag var n�jd b�rjade jag med att styla sidan.
Den absolut st�rsta tiden har jag lagt p� flexbox s� "designen" fick inte lika h�g prioritet, vilket kanske syns.
Hittade en f�rgkarta p� n�tet (http://bit.ly/2ADeQ7E) som jag utgick ifr�n. Det var sv�rt att f� texten l�sbar mot de olika f�rgerna s�
beslutade att ha en semi-tranparent vit bakgrund till all text. Tyv�rr g�r det att sidan blir lite v�l "fyrkantig" och "boxig", men l�sbarheten tyckte jag
var viktigare och jag fick en bra �vning i flexbox.
Fonten hittade jag p� Google Fonts. Den �r utan serifer vilket �ven det �kar l�sbarheten. 
Tyckte det var viktigt att fr�n b�rjan f�rs�ka f� sidan att passa i en mindre sk�rm, s� alla element �r stylade med relativa enheter som vh, vw, em osv.
Det �r inte perfekt �nnu men det fungerar delvis. Lyckades f� texten att skala ocks� med hj�lp av calc(px + vw) men jag vet inte riktigt om det 
�r "best practice".
Lade till kommentarer till min CSS som n�rmare f�rklarar de olika delarna.

Valde brytpunkt i media queries vid 768px som verkar vara vanligt vid anv�ndande av en iPad. Tanken med hela designen fr�n b�rjan var som sagt att inte beh�va massa media queries utan att beh�va �ndra s� lite som m�jligt.

<br>
<b>Validerade HTML och CSS och fick inga fel.</b>


"Document checking completed. No errors or warnings to show."


"W3C CSS-valideringsresultat f�r style.css (CSS niv� 3)

Gratulerar! Inga fel har hittats"
<br>
<br>
<br>
Feedback fr�n Victoria:

- <b>Du borde fr�mst anv�nda dig av relativa m�ttenheter: % och rem/em ist�llet px-v�rden. H�r finns en bra l�nk: 
https://www.w3schools.com/tags/ref_pxtoemconversion.asp</b>
	- Anv�nder mig fr�mst av relativa m�ttenheter. Enda g�ngen px anv�nds �r f�r att styra fontstorlek men d� anv�nds den tillsammans med vw i calc(px + vw) f�r att styra storlek p� font n�r sk�rmstorlek �ndras.

- <b>Det skulle vara bra om du lade till rubrikerna Home och About i sj�lva menyn s� man kan l�nka till de rubrikerna p� sidan.</b>
	- Har valt att inte g�ra det d� menyn inte f�ljer med n�r man skrollar p� sidan, allts� beh�vs inte Home. About tycker jag �r typ samma som Home, dvs �f�rstasidan�.

- <b>Det skulle vara bra att ha rubriker p� de olika delarna av sidan som menyn leder till t.ex. About, Themes, Pricing och Contact. Namn p� de olika rubrikerna kan l�ggas in i taggar av typen h2.</b>
	- Detta h�ll jag med om och har fixat! 

- <b>Det saknas namn p� f�retaget. Man kan l�gga in namnet i header med en tagg av typen h1.</b>
	- Det var ett medvetet val. F�retagsnamnet n�mns 3 g�nger �ver �hero-bilden� p� f�rstasidan vilket jag tycker r�cker gott och v�l.

- <b>Slogan borde flyttas fr�n footer till inneh�ller under rubriken About ist�llet. Du b�r inte anv�nda footer till slogan. Som alternativ kan du ist�llet anv�nda p tillsammans med strong eller endast h3.</b>
	- Gillar att slogan ligger l�ngst ner i footern. K�ndes on�digt att upprepa f�retagets adress d�r eller skriva n�gon konstig copyright-text. Bytte dock till h3.

- <b>Information om f�retaget kan man l�gga in i en p-tag ist�llet f�r h2. h2 passar j�ttebra f�r namn p� de olika rubrikerna.</b> 
	- Fixat!

- <b>Det skulle passa b�st om du anv�nder li till tabellen med priser ist�llet f�r p-taggar.</b>
	- Fixat!

- <b>Det ska vara bra om du anv�nder button f�r knappar ist�llet f�r p-taggar i Pris rubriken.</b>
	- Fixat!

- <b>Inputf�lten input type="submit"  i rubriken Contact saknar value="Submit".</b>
	- Fixat!

- <b>Priset f�r alternativet l�ngst till h�ger �r oj�mnt j�mf�rt de andra tv� alternativen. Det skulle se b�ttre ut om dessa l�g p� samma rad.</b>
	- Detta kunde jag f�r mitt liv inte fixa. S� det f�r ligga kvar som det �r.

- <b>Det �r b�ttre att l�gga rubriker som About,Themes och Pricing i section och deras sm� underrubriker i article ist�llet.</b> 
	- F�rst�r! Men jag f�ljde exemplet h�gts upp p� denna sida: https://www.w3schools.com/tags/tag_section.asp. S� jag tror att det g�r att anv�nda section-taggen p� det s�ttet som jag gjort.

- <b>Det �r b�ttre att l�gga in contact information(adressen,mail, sitemap,twitter och facebook) i footer ist�llet. H�r finns en bra l�nk https://www.w3schools.com/tags/tag_footer.asp</b>
	- Jag valde att l�gga kontaktinfo bredvid kontaktformul�ret ist�llet och ville inte upprepa samma info igen i footer. 

- <b>Det finns upprepande av egenskaper i CSS: color: #49654C; Det g�r att anv�nda sig av variabler f�r att �teranv�nda kod i CSS: 
https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables</b>
	- K�nner till det, men i det h�r fallet anv�nds bara 4 f�rger. S� tyckte inte det var n�dv�ndigt.

- <b>Anv�nd st�rre marginaler mellan de olika rubrikerna 
- Anv�nd st�rre padding f�r att g�ra k�nslan av sidan luftigare</b>  
	- Har �kat padding och margin n�got.