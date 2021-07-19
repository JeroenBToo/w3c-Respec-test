# Structuur 

## CAD-bestanden 

### Bestandsformaat 

Technisch revisietekenwerk wordt geleverd in een bestandsformaat dat
geopend, bewerkt en opgeslagen kan worden met het programma AutoCAD[2]:
het dwg-bestandsformaat (dwg-formaat). Bij deze handelingen in dit
softwarepakket mag er geen foutmelding optreden of informatie verloren
gaan. Afzonderlijk herkenbare entiteiten zijn in dit bestand ook als
zodanig gedefinieerd en door dit softwarepakket herkenbaar, zonder dat
daar extra verticale applicaties op zijn geïnstalleerd

(bijvoorbeeld: tekst is *text*,[3] lijnen zijn *lines* of *polylines*,
arceringen zijn *hatches*, maatvoeringen zijn *dimensions* en cirkels
zijn *circles*). Verder voldoen de bestanden aan de volgende
voorwaarden:

-   de bestanden zijn altijd gebaseerd op een metrisch *template*;

-   de bestanden zijn niet beveiligd door gebruik te maken van enige
    vorm van encryptie;

-   de bestanden bevatten geen ‘OLE-objecten’;

-   de bestanden bevatten geen *dictionaries*, behalve die door AutoCAD
    zélf automatisch worden gegenereerd;

-   de bestanden bevatten geen gerasterde entiteiten[4];

-   de bestanden bevatten geen, in het bestand geïntegreerde, *LISP-* of
    *VBA*-routines;

-   de bestanden bevatten geen entiteiten waaraan ‘hyperlinks’ gekoppeld
    zijn;

-   de bestanden bevatten geen entiteiten gegenereerd en ondersteund
    door *ObjectARX*-applicaties[5] (of: *proxy*-objecten), anders dan
    door AutoCAD zèlf automatisch gegenereerde (informatie over deze
    ‘add-ons’ is niet aanwezig en de samengestelde objecten zijn correct
    vertaald naar AutoCADbasisentiteiten en de koppeling naar de
    gebruikte ‘add-on’ is verbroken).

### Database koppelingen 

De CAD-bestanden[6] voor technisch revisietekenwerk bevatten geen
koppelingen naar externe databases[7]. Alle restinformatie binnen deze
CAD-bestanden, als gevolg van dergelijke 'databaseconnectivity' uit het
verleden, is niet meer aanwezig.

### Systeemvariabelen 

Binnen elk CAD-bestand zijn er *system variables* vastgelegd. Deze
systeemvariabelen zijn van invloed op diverse onderdelen binnen deze
bestanden. De systeemvariabelen hebben de waarden volgens de
onderstaande tabel.

<table>
<colgroup>
<col style="width: 54%" />
<col style="width: 45%" />
</colgroup>
<thead>
<tr class="header">
<th><em><strong>VARIABELE</strong></em></th>
<th><blockquote>
<p><em><strong>WAARDE</strong></em></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>LUNITS</td>
<td><blockquote>
<p>2</p>
</blockquote></td>
</tr>
<tr class="even">
<td>LWDISPLAY</td>
<td><blockquote>
<p>OFF</p>
</blockquote></td>
</tr>
<tr class="odd">
<td>MEASUREMENT</td>
<td><blockquote>
<p>1</p>
</blockquote></td>
</tr>
</tbody>
</table>

## Levering bronbestanden 

Volgens deze CAD Specificatie worden primair eisen gesteld aan door de
vervaardiger te leveren dwgen bijbehorende pdf-bestanden) . In het geval
deze bestanden zijn vervaardigd als extract uit bronbestanden geopend,
bewerkt en opgeslagen in software waarin het dwg-bestandsformaat niet
het eigen bestandsformaat is (bijvoorbeeld een BIM modelleerapplicatie),
dan worden de desbetreffende bronbestanden meegeleverd mét de
beschrijving van de wijze waarop deze extracten uit de bronbestanden
zijn gegenereerd.

## Basisprincipes voor technisch revisietekenwerk 

Technisch revisietekenwerk bestaat uit tweedimensionaal (2D) tekenwerk.
In deze paragraaf wordt nader ingegaan op de basisprincipes van
2D-tekenwerk volgens deze Specificatie.

### Projectievlak 

Bij het tweedimensionaal tekenen wordt gebruik gemaakt van een
projectievlak[8]. Het projectievlak is een virtueel vlak binnen of
buiten een bouwwerk waarin bouwdelen loodrecht geprojecteerd worden. In
het *WCS* in het CAD-bestand worden deze loodrechte projecties van
bouwdelen getekend. In het tekenwerk wordt uitsluitend gebruik gemaakt
van horizontale (bijvoorbeeld plattegronden) en verticale
projectievlakken (bijvoorbeeld doorsneden en gevels). Ten opzichte van
het projectievlak zijn er voor ieder [=bouwdeel=] drie mogelijke posities:

1.  <u>Achter/onder</u> het projectievlak: het componentaanzicht;

2.  <u>In</u> het projectievlak: de componentdoorsnijding;

3.  <u>Voor/boven</u> het projectievlak: de componentprojectie.

In een CAD-bestand is de positie van het projectievlak gedefinieerd en
de positie van componentaanzichten, -doorsnijdingen en -projecties ten
opzichte van dit projectievlak ondubbelzinnig afleesbaar.

Ter illustratie van dit basisprincipe wordt als voorbeeld de plattegrond
van de bovenste bouwlaag van een bouwwerk met een traditionele
kapconstructie gebruikt. Hieronder wordt een 3D-model van de kap van het
bouwwerk getoond en worden het bouwdeelaanzicht, de -doorsnijding en de
-projectie in de daarbij horende plattegrond getoond in de figuren 1, 2
en 3.

> <img src="media/image3.jpg" style="width:6.53743in;height:4.26623in" />

*Figuur 1: 3D-model van een kap*

<img src="media/image6.jpg" style="width:4.68681in;height:9.42301in" />*Figuur
2: projectievlak aangebracht: lichtgroen vlak voor bouwdeeldoorsnijding,
roze voor bouwdeelprojectie.*

<img src="media/image8.jpg" style="width:6.56736in;height:8.86597in" />

*Figuur 3: projectievlak aangebracht: lichtgeel vlak voor
bouwdeelaanzicht, lichtgroen voor bouwdeeldoorsnijding, roze voor
bouwdeelprojectie.*

Om in het CAD-bestand -en in de daarin aanwezige tekeningen- de positie
van bouwdelen ten opzichte van het projectievlak duidelijk herkenbaar te
maken, wordt er gebruik gemaakt van verschillende combinaties van
lijndikte, lijntype en arcering volgens de onderstaande tabel:

<table style="width:100%;">
<colgroup>
<col style="width: 25%" />
<col style="width: 33%" />
<col style="width: 21%" />
<col style="width: 18%" />
</colgroup>
<thead>
<tr class="header">
<th><em><strong>positie</strong></em></th>
<th><em><strong>lijndikte</strong></em></th>
<th><blockquote>
<p><em><strong>lijntype</strong></em></p>
</blockquote></th>
<th><em><strong>hatch</strong></em></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>bouwdeelaanzicht</td>
<td>kleiner dan doorsnijding</td>
<td><blockquote>
<p>getrokken lijn</p>
</blockquote></td>
<td>nee</td>
</tr>
<tr class="even">
<td>bouwdeeldoorsnijding</td>
<td>groter dan aanzicht en projectie</td>
<td><blockquote>
<p>getrokken lijn</p>
</blockquote></td>
<td><em>ja</em></td>
</tr>
<tr class="odd">
<td>bouwdeelprojectie</td>
<td>kleiner dan doorsnijding</td>
<td><blockquote>
<p>gestippeld</p>
</blockquote></td>
<td>nee</td>
</tr>
</tbody>
</table>

*Tabel 1: lijndikte, lijntype en arcering gekoppeld aan positie van
bouwdelen ten opzichte van het projectievlak*

> <img src="media/image9.png" style="width:6.47in;height:7.25667in" />

*Figuur 4: bouwdeelaanzicht (binnen gele uitsnede), bouwdeeldoorsnijding
(groene uitsnede) en bouwdeelprojectie (rode uitsnede) gesuperposeerd in
één plattegrond (binnen grijze uitsnede).*

### Plattegronden 

Plattegronden worden in beginsel beschouwd als een horizontale doorsnede
op 1200 mm boven het vloerpeil van de desbetreffende bouwlaag[9]. Deze
doorsnede is het projectievlak als bedoeld in § 1.3.1 Projectievlak.
CAD-bestanden met plattegronden moeten aan de volgende voorwaarden
voldoen:

-   elk CAD-bestand bevat slechts informatie met betrekking tot één
    bouwlaag;

-   bouwdeelaanzichten behorend bij de desbetreffende bouwlaag van een
    plattegrond worden volledig en gedetailleerd getekend (conform § 1.9
    Detailleringniveau);

-   zichtbare bouwdeelaanzichten behorend bij lager gelegen bouwlagen,
    worden schematisch getekend in een -bij visualisatie- dunne lijn;

-   in de plattegronden moet het projectievlak van aanwezige verticale
    doorsneden worden aangegeven met behulp van een doorsnedenaanduiding
    (bestaande uit een lijn die het projectievlak aangeeft, kijkrichting
    en een resulterende tweelettercode: bijvoorbeeld AA, BB enzovoort,
    hier staat A aan het begin van de lijn en A aan het eind van de
    lijn, steeds met een pijl die de kijkrichting aangeeft).

### Doorsneden 

Doorsneden worden beschouwd en getekend als een verticale doorsnede over
een deel van het bouwwerk[10]. Deze verticale doorsnede is het
projectievlak. Doorsneden moeten corresponderen met plattegronden en
gevels en vice versa. Eventueel aanwezige gevels van delen van het
bouwwerk in dit projectievlak moeten worden getekend conform de eisen
voor gevels.[11] In de bijbehorende plattegronden en doorsneden moet dit
projectievlak worden aangegeven met behulp van een doorsnedenaanduiding
(bestaande uit een lijn die het projectievlak aangeeft, kijkrichting en
een resulterende tweelettercode: bijvoorbeeld AA, BB enzovoort, hier
staat A aan het begin van de lijn en A aan het eind van de lijn, steeds
met een pijl die de kijkrichting aangeeft).

### Gevels 

Gevels worden beschouwd en getekend als een verticaal aanzicht van een
deel van het bouwwerk. Dit verticale aanzicht is het projectievlak.
Gevels moeten corresponderen met plattegronden en doorsneden en vice
versa. Gevelaanzichten worden in beginsel getekend als loodrechte
projecties van gevels op dit projectievlak. Eventueel aanwezige
doorsneden van delen van het bouwwerk in dit projectievlak moeten worden
getekend conform de eisen voor doorsneden.[12]

### Entiteiten getekend in het *WCS* 

Er worden in het projectievlak slechts één- en tweedimensionale
entiteiten getekend met een *elevation*, Z-waarde en een *thickness* van
0 (nul) in het *World Coördinate System* (*WCS*). Het tekenen van twee
of meer exact dezelfde entiteiten op dezelfde positie in het *WCS* is
niet toegestaan.

Voor visualisatiedoeleinden wordt slechts gebruik gemaakt van
onderscheid in de eigenschappen *color* (dikte van lijnen wordt slechts
gedefinieerd middels koppeling van lijndikten/pennen aan een specifieke
*color*) en *linetype* óf van onderscheid in *lineweight* en *linetype*.

## Informatiescheiding met behulp van *layers* 

Binnen een CAD-bestand moet informatie gescheiden worden. Dit vindt
plaats door verschillend geclassificeerde entiteiten te tekenen in
verschillende *layers*. Aan het gebruik van *layers* worden de volgende
basiseisen gesteld:

-   de loodrechte projecties van bouwdelen in het projectievlak worden
    getekend in verschillende *layers;*

-   de naam van de *layers* voor het tekenen van bouwdelen bevat de
    eerste twee cijfers van de

> NL/SfB elementcode (zonder haakje) van de elementgroep waartoe het
> [=bouwdeel=] behoort én de bijbehorende omschrijving, dit met de volgende
> syntax: \[NL/SfB elementcode\]\[spatie\]\[NL/SfB omschrijving\] (de
> elementgroepen zijn gedefinieerd in tabel 1 van de publicatie ‘NL/SfB
> tabellen 2005 inclusief herziene elementenmethode '91'[13]), de
> omschrijving bevat geen bijzondere karakters anders dan '-'
> (afbreekstreepje) of '\_' (laag liggend streepje);

-   er mogen geen *layers* voorkomen waarbinnen zich geen entiteiten
    bevinden (geen ‘lege’ *layers*), met uitzondering van *layer* **0**
    (nul);

-   in *layer* **0** (nul) mogen zich geen entiteiten bevinden anders
    dan meervoudige *blocks, viewports* of *external references*;

-   entiteiten worden slechts geplaatst in de daarvoor bedoelde
    *layers*;

-   in *layer* **defpoints** worden geen entiteiten geplaatst, anders
    dan de (hulp-)entiteiten die

AutoCAD automatisch genereert in deze *layer* bij het tekenen van
bijvoorbeeld een *dimension*;  bij oplevering van CAD-bestanden moet
*layer* **0** (nul) ingesteld worden als *current layer*.

## *Layout tabs* 

### Gebruik van *layout tabs* 

Binnen een CAD-bestand kunnen er verschillende *layout tabs* aangemaakt
worden. Het gebruik van *layout tabs* is aan de volgende regels
gebonden:

-   voor alle *layout tabs* geldt: 1 *drawing unit* = 1 millimeter;

-   binnen *modelspace* worden entiteiten altijd met schaal 1:1
    getekend;

-   bouwwerkgebonden entiteiten worden uitsluitend geplaatst in
    *modelspace* (in de *layout tab*

> *Model*); tekeninggebonden entiteiten komen hier niet in voor;

-   tekeninggebonden entiteiten worden uitsluitend geplaatst in
    *paperspace*; bouwwerkgebonden entiteiten komen hier niet in voor;

-   binnen een CAD-bestand is tenminste één tekening gedefinieerd;

-   binnen een *layout tab* (anders dan de *layout tab* *Model*) is er
    maximaal één tekening gedefinieerd.

### Naamgeving van *layout tabs* 

Er worden geen eisen gesteld aan de naamgeving van *layout-tabs*.

## *Paperspace* 

### Tekeningkader en titelblok 

Een tekening wordt uitsluitend geplaatst in een layout-tab in de
*paperspace* van een CAD-bestand, deze *layout tabs* bevatten elk
slechts één tekening. Binnen een CAD-bestand is tenminste één tekening
gedefinieerd. In een tekening zijn binnen het tekeningkader één of meer
viewports gedefinieerd waarbinnen (al dan niet verschaald) de
*modelspace* zichtbaar is. Een CAD-bestand waarin meerdere tekeningen
zijn gedefinieerd heeft betrekking op slechts één discipline of aspect.
Als er meerdere tekeningen gedefinieerd zijn binnen een CAD-bestand, dan
hebben alle tekeningen in het titelblok één hoofdonderwerp[14] wat de
inhoud van alle tekeningen beschrijft. Naast het hoofdonderwerp heeft
elke tekening een sub-onderwerp wat de inhoud van de individuele
tekening beschrijft.

### Gebruik van *blocks* 

Gebruik en plaatsing van *blocks* in de *paperspace* van een CAD-bestand
is toegestaan. Slechts verzamelingen van entiteiten die meer dan één
keer voorkomen in het revisietekenwerk binnen één project mogen worden
gedefinieerd als een *block*.

### Naamgeving van *blocks* 

Namen van *blocks* zijn gesteld in de Nederlandse of Engelse taal.

### Gebruik van *external references* 

Gebruik van *external references* in de *paperspace* van een CAD-bestand
is niet toegestaan.

### Tekeninggebonden tekst 

Tekeninggebonden tekst wordt geplaatst in een daarvoor geëigende
*layer*.

## *Modelspace* 

### Gebruik van *blocks* 

Gebruik en plaatsing van *blocks* in de *modelspace* van een CAD-bestand
is toegestaan. Slechts verzamelingen van entiteiten die meer dan één
keer voorkomen in het revisietekenwerk binnen één project mogen worden
gedefinieerd als een *block*.

### Naamgeving van *blocks* 

Namen van blocks zijn gesteld in de Nederlandse of Engelse taal.

### Gebruik van *external references* 

Gebruik van *external references* moet voldoen aan alle volgende
voorwaarden:

-   een *external reference* is altijd een bestand binnen de discipline
    Bouwkunde met een plattegrond,

-   er zijn geen *external references* waarbinnen geen tekening is
    gedefinieerd;

-   relaties met *external reference*-bestanden in *master*-bestanden
    zijn altijd van het type *attached*[15], een *external reference* is
    altijd een *attached reference*;

-   het ‘saved path’ in *master*-bestanden naar een *external
    reference*–bestand bevat alleen de bestandsnaam van het een
    *external reference*–bestand;

-   er ontstaat geen kringverwijzing in CAD-bestanden behorend tot de
    verzameling revisietekenwerkbestanden onder één project;

-   *Een external reference* wordt altijd geplaatst in *layer* **0**
    (nul).

### Positie bouwwerk 

Het getekende bouwwerk in een CAD-bestand bevindt zich volledig binnen
het 1e kwadrant van het *WCS*, met de linker onderhoek van het bouwwerk
nabij de oorsprong.

### Stramien 

Voor het definiëren van stramienen in een tekening is NEN 2302:1983 (§
4.1) van toepassing.

### Hoogtematen 

Voor het aangeven van hoogtematen in een tekening is NEN 2302:1983 van
toepassing (§ 5.3.2), tenzij elders binnen deze Specificatie anders of
specifieker is omschreven. Hoogtematen worden gesteld in millimeters.
Hoogtematen worden altijd aangegeven in millimeters boven (+) of onder
(-) het vastgestelde peil. Hoogtematen van bovenzijden[16] van
horizontale vlakken worden in deze Specificatie peilmaat genoemd.

### Maataanduiding 

Voor maataanduidingen binnen CAD-bestanden mag geen gebruik gemaakt
worden van *text overrides* om, bijvoorbeeld, maatafwijkingen in
getekende bouwdelen te corrigeren. Het veld *text override* in de
*properties-toolbar* (bij selectie van een *dimension*) moet leeg zijn.
Voor de tekenwijze van maataanduidingen in een tekening is, tenzij
elders binnen deze Specificatie anders of specifieker omschreven, NEN
2302:1983 (hoofdstuk 5; inclusief de in 5.1.1 aangegeven voorkeuren) van
toepassing.

### Bouwwerkgebonden tekst 

Bouwwerkgebonden tekst wordt geplaatst in een *layer* voor tekst
behorend bij de desbetreffende NL/SfB elementcode,

## Tekeningsoort 

Technisch revisietekenwerk is opgebouwd conform NPR 2570:1986, hoofdstuk
2 en kan bestaan uit de tekeningsoorten zoals gedefinieerd in NPR
2570:1986, hoofdstuk 2.

## Detailleringniveau 

Het detailleringniveau van technisch revisietekenwerk moet minimaal
voldoen aan de eisen voor tekenwerk uit de fase 'bestek' zoals
gedefinieerd in NEN 2574:1993, tenzij elders binnen deze Specificatie
anders of specifieker omschreven.

## Nauwkeurigheid 

Bouwdelen worden volledig, nauwkeurig en herkenbaar getekend en
gerepresenteerd met behulp van entiteiten.

Entiteiten die bouwdelen representeren die binnen het bouwwerk
aanliggend of opliggend zijn, dienen ook zodanig getekend te zijn binnen
het CAD-bestand: bij een vergrotingsfactor van 1000 dienen dergelijke
entiteiten nog steeds aanliggend of opliggend te zijn en bij herhaald
gebruik van de *object snap* functies dient steeds hetzelfde
snapresultaat te ontstaan.

Entiteiten die bouwdelen representeren die binnen bouwwerken loodrecht
ten opzichte van elkaar gepositioneerd zijn, dienen ook zodanig getekend
te zijn binnen het CAD-bestand: na bijtekenen van loodrechte hulplijnen
op het (denkbeeldige) snijpunt van de entiteiten dienen bij een
vergrotingsfactor van 1000 dergelijke entiteiten en de hulplijnen nog
steeds aanliggend of opliggend te zijn en bij herhaald gebruik van de
*object snap* functies dient steeds hetzelfde snapresultaat te ontstaan.

## Bouwlaagaanduiding 

Aanduiding van bouwlagen vindt op zodanige wijze plaats dat
ondubbelzinnig duidelijk is hoe de verschillende bouwlagen in een
bouwwerk ten opzichte van elkaar gelegen zijn in verticale zin. Dit
gebeurt met de aanduiding \<Bouwlaagnummer>\<spatie>\<Bouwlaagtekst>.
Hierbij geldt:

-   \<Bouwlaagnummer> is verplicht en bestaat uit twee karakterposities
    voor het bouwlaaghoofdnummer:..., -2, -1, 00, 01, 02, ... Hierin is
    -1 de eerste kelderbouwlaag, 00 de bouwlaag met de dominante
    hoofdtoegang en 01 het nummer voor een hoger gelegen bouwlaag. Bij
    een tussenverdieping krijgt het bouwlaaghoofdnummer een toevoeging
    met 1 karakterpositie met een letter voor aanduiding van de
    tussenverdieping. Als er binnen eenzelfde bouwlaaghoofdnummer
    meerdere tussenverdiepingen zijn, worden deze met een alfabetisch
    opeenvolgende letter aangeduid: bijvoorbeeld 00t, 00s (een letter
    met een eerdere positie in het alfabet duidt daarbij een lager
    gelegen tussenverdieping aan).

-   \<Bouwlaagtekst> is optioneel en is een tekstuele beschrijving, al
    of niet voorafgegaan door een rangtelwoord.

## Constructie (discipline) 

Binnen deze discipline zijn er nog geen specifieke structuureisen van
kracht anders dan in algemene zin in deze Specificatie beschreven. Het
wettelijk kader is hiervoor eerste uitgangspunt.

## Bouwkunde (discipline) 

Binnen deze discipline zijn er nog geen specifieke structuureisen van
kracht anders dan in algemene zin in deze Specificatie beschreven. Het
wettelijk kader is hiervoor eerste uitgangspunt.

## Werktuigbouw (discipline) 

Binnen deze discipline zijn er nog geen specifieke structuureisen van
kracht anders dan in algemene zin in deze Specificatie beschreven. Het
bestaande wettelijk kader is hiervoor eerste uitgangspunt.

## Elektrotechniek (discipline) 

Binnen deze discipline zijn er nog geen specifieke structuureisen van
kracht anders dan in algemene zin in deze Specificatie beschreven. Het
bestaande wettelijk kader is hiervoor eerste uitgangspunt.

## Terrein (discipline) 

Binnen deze discipline zijn er nog geen specifieke structuureisen van
kracht anders dan in algemene zin in deze Specificatie beschreven. Het
bestaande wettelijk kader is hiervoor eerste uitgangspunt.

## Brandveiligheid (aspect) 

Tekeningen voor het aspect brandveiligheid voldoen aan de volgende
aanvullende structuureisen:

-   de corresponderende bouwkundige tekening is als ‘onderlegger’
    toegevoegd en als *block* geplaatst op *layer* **0**;

-   alle getekende brandveiligheidsinformatie conformeert zich aan NEN
    1413:2011;

-   alle getekende brandveiligheidsinformatie, zoals symbolen en lijnen,
    is geplaatst op de *layer* met NL/SfB-elementcode 65;

-   ieder symbool (met uitzondering van compartimentlijnen) bestaat uit
    een *block* met de inhoud en eigenschappen zoals voorgeschreven in
    NEN 1413:2011.

## Beveiliging (aspect) 

Binnen dit aspect zijn er nog geen specifieke structuureisen van kracht
anders dan in algemene zin in deze Specificatie beschreven. Het
bestaande wettelijk kader is hiervoor eerste uitgangspunt.

