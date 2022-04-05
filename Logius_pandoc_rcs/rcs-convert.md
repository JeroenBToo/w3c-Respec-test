# Voorwoord

Het Rijksvastgoedbedrijf is de vastgoedorganisatie van en voor de
Rijksoverheid. Het Rijksvastgoedbedrijf is verantwoordelijk voor
instandhouding en beheer van de grootste en meest diverse
vastgoedportefeuille van Nederland. Het Rijksvastgoedbedrijf treedt
vanuit zijn rol veelal op als eindopdrachtgever. Voor een adequaat
beheer van de portefeuille is actuele vastgoedinformatie noodzakelijk.
Vastgoedinformatie wordt vaak vastgelegd in tekeningen, naast andere
wijzen van vastlegging. Bij nieuwbouw, verbouw, aankoop, aanhuur en
onderhoud van bouwwerken worden tekeningen geraadpleegd en vervaardigd.
Vooral tekeningen waarop de gerealiseerde situatie ter plaatse wordt
weergegeven -technisch revisietekenwerk of 'as built'/’as is’/'as
maintained' tekenwerk- zijn voor het Rijksvastgoedbedrijf van belang.
Het Rijksvastgoedbedrijf stelt met deze CAD Specificatie[^1] eisen aan
dit technisch revisietekenwerk.

Het Rijksvastgoedbedrijf behoudt zich het recht voor om in concrete
gevallen aanvullende of afwijkende instructies (aanvullend of afwijkend
ten opzichte van deze Specificatie) af te geven voor vervaardiging van
technisch revisietekenwerk.

Op diverse plaatsen in deze Specificatie wordt er verwezen naar externe
normen. Als er in deze Specificatie aanvullende of afwijkende eisen
(aanvullend of afwijkend ten opzichte van deze externe normen) worden
gesteld dan gaan deze altijd vóór op het bepaalde in deze externe
normen. De eisen zijn van toepassing op alle revisietekenwerk binnen een
project en gelden voor alle disciplines. Als er voor een discipline
aanvullende en/of afwijkende eisen gesteld worden, wordt dit specifiek
aangegeven

<img src=".//media/image7.png"
style="width:3.08472in;height:2.91944in" />Leeswijzer

Technisch revisietekenwerk wordt geleverd in een CAD-bestand.
CAD-bestanden zijn te beschrijven in vier dimensies: structuur, inhoud,
visualisatie en opslag. Bij structuur gaat het om de samenhang, en
daarmee de betekenis, van de entiteiten aangebracht binnen een
CAD-bestand. Bij inhoud gaat het om het vastleggen van de werkelijkheid
met behulp van deze gestructureerde en betekenisvolle entiteiten. Bij
visualisatie gaat het om de vertaling van de aangebrachte inhoud en
structuur in een CAD-bestand naar een ander medium voor ter
beschikkingstelling van de informatie. Bij opslag gaat het om de opslag
van een CAD-bestand. Voor elke dimensie zijn er in deze Specificatie
eisen opgesteld.

De hoofdstukken 1 tot en met 4 beschrijven de eisen voor technisch
revisietekenwerk met betrekking tot deze vier dimensies. In de bijlagen
komen achtereenvolgend definities, tekeningenlijst en normenoverzicht
aan bod.

# Structuur

## CAD-bestanden

### Bestandsformaat

Technisch revisietekenwerk wordt geleverd in een bestandsformaat dat
geopend, bewerkt en opgeslagen kan worden met het programma AutoCAD[^2]:
het dwg-bestandsformaat (dwg-formaat). Bij deze handelingen in dit
softwarepakket mag er geen foutmelding optreden of informatie verloren
gaan. Afzonderlijk herkenbare entiteiten zijn in dit bestand ook als
zodanig gedefinieerd en door dit softwarepakket herkenbaar, zonder dat
daar extra verticale applicaties op zijn geïnstalleerd (bijvoorbeeld:
tekst is *text*,[^3] lijnen zijn *lines* of *polylines*, arceringen zijn
*hatches*, maatvoeringen zijn *dimensions* en cirkels zijn *circles*).
Verder voldoen de bestanden aan de volgende voorwaarden:

-   de bestanden zijn altijd gebaseerd op een metrisch *template*;

-   de bestanden zijn niet beveiligd door gebruik te maken van enige
    vorm van encryptie;

-   de bestanden bevatten geen ‘OLE-objecten’;

-   de bestanden bevatten geen *dictionaries*, behalve die door AutoCAD
    zélf automatisch worden gegenereerd;

-   de bestanden bevatten geen gerasterde entiteiten[^4];

-   de bestanden bevatten geen, in het bestand geïntegreerde, *LISP-* of
    *VBA*-routines;

-   de bestanden bevatten geen entiteiten waaraan ‘hyperlinks’ gekoppeld
    zijn;

-   de bestanden bevatten geen entiteiten gegenereerd en ondersteund
    door *ObjectARX*-applicaties[^5] (of: *proxy*-objecten), anders dan
    door AutoCAD zèlf automatisch gegenereerde (informatie over deze
    ‘add-ons’ is niet aanwezig en de samengestelde objecten zijn correct
    vertaald naar AutoCAD-basisentiteiten en de koppeling naar de
    gebruikte ‘add-on’ is verbroken).

### Database koppelingen

De CAD-bestanden[^6] voor technisch revisietekenwerk bevatten geen
koppelingen naar externe databases[^7]. Alle restinformatie binnen deze
CAD-bestanden, als gevolg van dergelijke 'database-connectivity' uit het
verleden, is niet meer aanwezig.

### Systeemvariabelen

Binnen elk CAD-bestand zijn er *system variables* vastgelegd. Deze
systeemvariabelen zijn van invloed op diverse onderdelen binnen deze
bestanden. De systeemvariabelen hebben de waarden volgens de
onderstaande tabel.

| VARIABELE   | WAARDE |
|-------------|--------|
| LUNITS      | 2      |
| LWDISPLAY   | OFF    |
| MEASUREMENT | 1      |

## Levering bronbestanden

Volgens deze CAD Specificatie worden primair eisen gesteld aan door de
vervaardiger te leveren dwg-en bijbehorende pdf-bestanden) . In het
geval deze bestanden zijn vervaardigd als extract uit bronbestanden
geopend, bewerkt en opgeslagen in software waarin het
dwg-bestandsformaat niet het eigen bestandsformaat is (bijvoorbeeld een
BIM modelleerapplicatie), dan worden de desbetreffende bronbestanden
meegeleverd mét de beschrijving van de wijze waarop deze extracten uit
de bronbestanden zijn gegenereerd.

## Basisprincipes voor technisch revisietekenwerk

Technisch revisietekenwerk bestaat uit tweedimensionaal (2D) tekenwerk.
In deze paragraaf wordt nader ingegaan op de basisprincipes van
2D-tekenwerk volgens deze Specificatie.

### Projectievlak

Bij het tweedimensionaal tekenen wordt gebruik gemaakt van een
projectievlak[^8]. Het projectievlak is een virtueel vlak binnen of
buiten een bouwwerk waarin bouwdelen loodrecht geprojecteerd worden. In
het *WCS* in het CAD-bestand worden deze loodrechte projecties van
bouwdelen getekend. In het tekenwerk wordt uitsluitend gebruik gemaakt
van horizontale (bijvoorbeeld plattegronden) en verticale
projectievlakken (bijvoorbeeld doorsneden en gevels). Ten opzichte van
het projectievlak zijn er voor ieder bouwdeel drie mogelijke posities:

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

| <img src=".//media/image8.png" style="width:3.14931in;height:4.23889in" 
 alt="090501 BRT-B fig-01a" />                                            | <img src=".//media/image9.png" style="width:3.25347in;height:2.05972in"  
                                                                           alt="090501 BRT-B fig-01b" />                                             |
|-------------------------------------------------------------------------|--------------------------------------------------------------------------|
|                                                                         | <img src=".//media/image10.png" style="width:3.25347in;height:2.07431in" 
                                                                           alt="090501 BRT-B fig-01c" />                                             |

Figuur 1: 3D-model van een kap

| <img src=".//media/image11.png" style="width:4.67153in;height:4.68681in" 
 alt="090501 BRT-B fig-02a" />                                             |
|--------------------------------------------------------------------------|
| <img src=".//media/image12.png" style="width:4.68681in;height:4.70139in" 
 alt="090501 BRT-B fig-02b" />                                             |

Figuur 2: projectievlak aangebracht: lichtgroen vlak voor
bouwdeeldoorsnijding, roze voor bouwdeelprojectie.

<img src=".//media/image13.png" style="width:6.56736in;height:8.86597in"
alt="090501 BRT-B fig-03" />

Figuur 3: projectievlak aangebracht: lichtgeel vlak voor
bouwdeelaanzicht, lichtgroen voor bouwdeeldoorsnijding, roze voor
bouwdeelprojectie.

Om in het CAD-bestand -en in de daarin aanwezige tekeningen- de positie
van bouwdelen ten opzichte van het projectievlak duidelijk herkenbaar te
maken, wordt er gebruik gemaakt van verschillende combinaties van
lijndikte, lijntype en arcering volgens de onderstaande tabel:

| positie              | lijndikte                        | lijntype       | hatch |
|----------------------|----------------------------------|----------------|-------|
| bouwdeelaanzicht     | kleiner dan doorsnijding         | getrokken lijn | nee   |
| bouwdeeldoorsnijding | groter dan aanzicht en projectie | getrokken lijn | *ja*  |
| bouwdeelprojectie    | kleiner dan doorsnijding         | gestippeld     | nee   |

Tabel 1: lijndikte, lijntype en arcering gekoppeld aan positie van
bouwdelen ten opzichte van het projectievlak

| <img src=".//media/image14.wmf" style="width:2.16389in;height:2.19375in" 
 alt="090501 BRT-B fig-04a" />                                             | <img src=".//media/image15.wmf" style="width:2.07431in;height:2.20903in" 
                                                                            alt="090501 BRT-B fig-04b" />                                             | <img src=".//media/image16.wmf" style="width:2in;height:2.23889in" 
                                                                                                                                                       alt="090501 BRT-B fig-04c" />                                       |
|--------------------------------------------------------------------------|--------------------------------------------------------------------------|--------------------------------------------------------------------|
| <img src=".//media/image17.wmf" style="width:5in;height:5.05972in"       
 alt="090501 BRT-B fig-04d" />                                             |                                                                          |                                                                    |

Figuur 4: bouwdeelaanzicht (binnen gele uitsnede), bouwdeeldoorsnijding
(groene uitsnede) en bouwdeelprojectie (rode uitsnede) gesuperposeerd in
één plattegrond (binnen grijze uitsnede).

### Plattegronden

Plattegronden worden in beginsel beschouwd als een horizontale doorsnede
op 1200 mm boven het vloerpeil van de desbetreffende bouwlaag[^9]. Deze
doorsnede is het projectievlak als bedoeld in § . CAD-bestanden met
plattegronden moeten aan de volgende voorwaarden voldoen:

-   elk CAD-bestand bevat slechts informatie met betrekking tot één
    bouwlaag;

-   bouwdeelaanzichten behorend bij de desbetreffende bouwlaag van een
    plattegrond worden volledig en gedetailleerd getekend (conform § );

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
een deel van het bouwwerk[^10]. Deze verticale doorsnede is het
projectievlak. Doorsneden moeten corresponderen met plattegronden en
gevels en vice versa. Eventueel aanwezige gevels van delen van het
bouwwerk in dit projectievlak moeten worden getekend conform de eisen
voor gevels.[^11] In de bijbehorende plattegronden en doorsneden moet
dit projectievlak worden aangegeven met behulp van een
doorsnedenaanduiding (bestaande uit een lijn die het projectievlak
aangeeft, kijkrichting en een resulterende tweelettercode: bijvoorbeeld
AA, BB enzovoort, hier staat A aan het begin van de lijn en A aan het
eind van de lijn, steeds met een pijl die de kijkrichting aangeeft).

### Gevels

Gevels worden beschouwd en getekend als een verticaal aanzicht van een
deel van het bouwwerk. Dit verticale aanzicht is het projectievlak.
Gevels moeten corresponderen met plattegronden en doorsneden en vice
versa. Gevelaanzichten worden in beginsel getekend als loodrechte
projecties van gevels op dit projectievlak. Eventueel aanwezige
doorsneden van delen van het bouwwerk in dit projectievlak moeten worden
getekend conform de eisen voor doorsneden.[^12]

### Entiteiten getekend in het ***WCS***

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
    eerste twee cijfers van de NL/SfB elementcode (zonder haakje) van de
    elementgroep waartoe het bouwdeel behoort én de bijbehorende
    omschrijving, dit met de volgende syntax: \[NL/SfB
    elementcode\]\[spatie\]\[NL/SfB omschrijving\] (de elementgroepen
    zijn gedefinieerd in tabel 1 van de publicatie ‘NL/SfB tabellen 2005
    inclusief herziene elementenmethode '91'[^13]), de omschrijving
    bevat geen bijzondere karakters anders dan '-' (afbreekstreepje) of
    '\_' (laag liggend streepje);

-   er mogen geen *layers* voorkomen waarbinnen zich geen entiteiten
    bevinden (geen ‘lege’ *layers*), met uitzondering van *layer* **0**
    (nul);

-   in *layer* **0** (nul) mogen zich geen entiteiten bevinden anders
    dan meervoudige *blocks, viewports* of *external references*;

-   entiteiten worden slechts geplaatst in de daarvoor bedoelde
    *layers*;

-   in *layer* **defpoints** worden geen entiteiten geplaatst, anders
    dan de (hulp-)entiteiten die AutoCAD automatisch genereert in deze
    *layer* bij het tekenen van bijvoorbeeld een *dimension*;

-   bij oplevering van CAD-bestanden moet *layer* **0** (nul) ingesteld
    worden als *current layer*.

## *Layout tabs*

### Gebruik van ***layout tabs***

Binnen een CAD-bestand kunnen er verschillende *layout tabs* aangemaakt
worden. Het gebruik van *layout tabs* is aan de volgende regels
gebonden:

-   voor alle *layout tabs* geldt: 1 *drawing unit* = 1 millimeter;

-   binnen *modelspace* worden entiteiten altijd met schaal 1:1
    getekend;

-   bouwwerkgebonden entiteiten worden uitsluitend geplaatst in
    *modelspace* (in de *layout tab* *Model*); tekeninggebonden
    entiteiten komen hier niet in voor;

-   tekeninggebonden entiteiten worden uitsluitend geplaatst in
    *paperspace*; bouwwerkgebonden entiteiten komen hier niet in voor;

-   binnen een CAD-bestand is tenminste één tekening gedefinieerd;

-   binnen een *layout tab* (anders dan de *layout tab* *Model*) is er
    maximaal één tekening gedefinieerd.

### Naamgeving van ***layout tabs***

Er worden geen eisen gesteld aan de naamgeving van *layout-tabs*.

##  *Paperspace*

### Tekeningkader en titelblok

Een tekening wordt uitsluitend geplaatst in een layout-tab in de
*paperspace* van een CAD-bestand, deze *layout tabs* bevatten elk
slechts één tekening. Binnen een CAD-bestand is tenminste één tekening
gedefinieerd. In een tekening zijn binnen het tekeningkader één of meer
viewports gedefinieerd waarbinnen (al dan niet verschaald) de
*modelspace* zichtbaar is. Een CAD-bestand waarin meerdere tekeningen
zijn gedefinieerd heeft betrekking op slechts één discipline of aspect.
Als er meerdere tekeningen gedefinieerd zijn binnen een CAD-bestand, dan
hebben alle tekeningen in het titelblok één hoofdonderwerp[^14] wat de
inhoud van alle tekeningen beschrijft. Naast het hoofdonderwerp heeft
elke tekening een sub-onderwerp wat de inhoud van de individuele
tekening beschrijft.

### Gebruik van ***blocks***

Gebruik en plaatsing van *blocks* in de *paperspace* van een CAD-bestand
is toegestaan. Slechts verzamelingen van entiteiten die meer dan één
keer voorkomen in het revisietekenwerk binnen één project mogen worden
gedefinieerd als een *block*.

### Naamgeving van ***blocks***

Namen van *blocks* zijn gesteld in de Nederlandse of Engelse taal.

### Gebruik van ***external references***

Gebruik van *external references* in de *paperspace* van een CAD-bestand
is niet toegestaan.

### Tekeninggebonden tekst

Tekeninggebonden tekst wordt geplaatst in een daarvoor geëigende
*layer*.

## *Modelspace*

### Gebruik van ***blocks***

Gebruik en plaatsing van *blocks* in de *modelspace* van een CAD-bestand
is toegestaan. Slechts verzamelingen van entiteiten die meer dan één
keer voorkomen in het revisietekenwerk binnen één project mogen worden
gedefinieerd als een *block*.

### Naamgeving van ***blocks***

Namen van blocks zijn gesteld in de Nederlandse of Engelse taal.

### Gebruik van ***external references***

Gebruik van *external references* moet voldoen aan alle volgende
voorwaarden:

-   een *external reference* is altijd een bestand binnen de discipline
    Bouwkunde met een plattegrond,

-   er zijn geen *external references* waarbinnen geen tekening is
    gedefinieerd;

-   relaties met *external reference*-bestanden in *master*-bestanden
    zijn altijd van het type *attached*[^15], een *external reference*
    is altijd een *attached reference*;

-   het ‘saved path’ in *master*-bestanden naar een *external
    reference*–bestand bevat alleen de bestandsnaam van het een
    *external reference*–bestand;

-   er ontstaat geen kringverwijzing in CAD-bestanden behorend tot de
    verzameling revisietekenwerk-bestanden onder één project;

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
(-) het vastgestelde peil. Hoogtematen van bovenzijden[^16] van
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
gebeurt met de aanduiding \<Bouwlaagnummer\>\<spatie\>\<Bouwlaagtekst\>.
Hierbij geldt:

-   \<Bouwlaagnummer\> is verplicht en bestaat uit twee karakterposities
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

-   \<Bouwlaagtekst\> is optioneel en is een tekstuele beschrijving, al
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

# Inhoud

## Basiseisen voor inhoud

Technisch revisietekenwerk wordt veelal geleverd in het kader van een
project voor de realisatie van nieuwbouw, verbouw, aankoop, aanhuur en
onderhoud van bouwwerken. Het Rijksvastgoedbedrijf treedt vanuit zijn
rol in de realisatie en instandhouding van huisvesting veelal op als
eindopdrachtgever van een dergelijk project. Aan het technisch
revisietekenwerk conform deze Specificatie worden de volgende algemene
inhoudseisen gesteld:

-   in het tekenwerk wordt de gerealiseerde situatie ter plaatse
    weergegeven: de 'as built'/’as is’/'as maintained' situatie;

-   alle getekende informatie ten behoeve van de
    realisatie/montage/installatie van bouwdelen wordt eveneens getekend
    in het bijbehorende technisch revisietekenwerk;

-   alle in het project gerealiseerde bouwdelen binnen elke discipline
    worden volledig getekend/gerepresenteerd volgens de principes in § ;

-   aangeboden CAD-bestanden met technisch revisietekenwerk mogen
    slechts informatie bevatten van één Bouwwerkcode; als binnen het
    werk meerdere Bouwwerkcodes onder handen én met elkaar verbonden
    zijn, is opnemen van Bouwwerkinformatie van meerdere Bouwwerkcodes
    in één CAD-bestand slechts toegestaan na overleg met en na
    schriftelijke toestemming mét nadere instructie van de
    RVB-opdrachtgever;

-   bij verbouw van bouwwerken en/of vervanging van bouwdelen van
    bouwwerken wordt het getekende uit het bestaande (door het RVB
    aangeleverde) technisch revisietekenwerk volledig inhoudelijk
    overgenomen, worden de wijzigingen getekend en wordt in het
    geactualiseerde technisch revisietekenwerk aangegeven welke
    gebieden/bouwdelen zijn gewijzigd ten opzichte van dat bestaande
    (door het RVB aangeleverde) technisch revisietekenwerk;

-   de getekende informatie in het technisch revisietekenwerk van een
    project wordt in een zo beperkt mogelijke set tekeningen vastgelegd;

-   de getekende informatie is zo min mogelijk redundant, het principe
    van éénmalige vastlegging en meermalig gebruik wordt maximaal
    toegepast;

-   de getekende informatie in de volledige set technisch
    revisietekenwerk van een project is niet onderling strijdig;

-   van alle bouwlagen is een plattegrond getekend en is er daarmee van
    alle ruimten een plattegrond getekend.

-   alle kenmerkende doorsneden zijn getekend: alle doorsneden met
    hoogteverschillen in peilmaten van ruimten, trappen, vides en die
    waaruit de verticale samenhang blijkt;

-   alle gevels zijn getekend, ook binnengevels (eventueel als onderdeel
    van doorsneden).

    In de hiernavolgende paragrafen worden per discipline nadere eisen
    gesteld.

## Constructie (discipline)

Alle in het project gerealiseerde bouwdelen binnen deze discipline
worden getekend. Het wettelijk kader is hierbij eerste uitgangspunt.
Minimaal gaat het om het tekenen van de volgende bouwdelen en/of
weergave van eigenschappen:

-   alle bouwdelen van de hoofddraagconstructie;

-   het onderscheid tussen geprefabriceerd en in het werk gestort beton;

-   toegepaste betonkwaliteiten en staalsoorten;

-   tijdsduur tot bezwijken, indien bepaald tijdens het ontwerpen van
    bouwdelen of materialen;

-   overspanningsrichting.

## Bouwkunde (discipline)

### Basis bouwdeelniveau Bouwkunde

Alle in het project gerealiseerde bouwdelen binnen deze discipline
worden getekend. Het bestaande wettelijk kader is hiervoor eerste
uitgangspunt. Minimaal gaat het om het tekenen van de volgende bouwdelen
en/of weergave van eigenschappen:

-   wanden, vloeren en daken; inclusief de plaatselijke onderbrekingen
    daarin (vides, sparingen enzovoort);

-   wandafwerkingen voorzien van een attest of certificaat, inclusief
    materiaalaanduiding (de tekst in het renvooi komt overeen met de
    materiaalnaam of aanduiding in het attest of certificaat);

-   wand- vloer- en dakopeningen (deuren, ramen, luiken, daklichten,
    rook-/warmteafvoeren enzovoort), inclusief weergave van
    openingsrichting (draaicirkelboog) en bewegingsvlak.

-   verticale verkeersvoorzieningen (trappen, hellingen, liften
    enzovoort) en is -indien van toepassing- voorzien van een pijl in de
    stijgrichting;

-   balustraden en leuningen;

-   vaste voorzieningen (keukens, sanitair, inbouwkasten enzovoort).

### Stramien

Alle projecties zijn voorzien van een stramien waarmee een referentie
ontstaat voor plaatsbepaling van bouwdelen. Het stramien wordt volledig
getekend in alle plattegronden.

### Hoogtematen

De peilmaten van elk vloerveld, boven (+) of onder (-) het vastgestelde
peil, worden aangegeven in alle voorkomende projecties.

### Maataanduiding

Minmaal de volgende maataanduidingen moeten zijn aangebracht in een
CAD-bestand:

-   stramienen (in alle projecties), voor zover van toepassing;

-   uitwendige maten van bouwwerken (in alle projecties);

-   netto hoogtematen van verdiepingen met tussenliggende en
    totaalmaten, ten opzichte van het vastgestelde peil, in doorsneden;

-   hoofdgevelmaten, goothoogten en nokhoogten, ten opzichte van het
    vastgestelde peil, in gevels.

### Ruimtenaam

Elke ruimte binnen een bouwwerk wordt voorzien van minimaal één naam. De
ruimtenaam wordt weergegeven in de vorm van tekst geplaatst in de
plattegrond van de getekende ruimte in een *layer* voor tekst volgens
tabel 0 van de publicatie ‘NL/SfB tabellen 2005 inclusief herziene
elementenmethode '91'[^17]. Het gaat bij de ruimtenaam om een
beschrijving van de (gebruikers-)activiteiten die plaatsvinden in een
ruimte[^18].

### Ruimtecode

Elke ruimte binnen een bouwwerk wordt voorzien van een unieke code in de
vorm van tekst geplaatst in de plattegrond van de getekende ruimten in
een *layer* voor tekst volgens tabel 0 van de publicatie ‘NL/SfB
tabellen 2005 inclusief herziene elementenmethode '91'[^19].

## Werktuigbouw (discipline)

Alle in het project gerealiseerde bouwdelen binnen deze discipline
worden getekend. Het bestaande wettelijk kader is hiervoor eerste
uitgangspunt. Minimaal gaat het om het tekenen van de volgende bouwdelen
en/of weergave van eigenschappen:

-   brandkleppen;

-   brandafsluiters in een W-installatie ter plaatse van een
    compartimentdoorvoer;

-   (nood)afsluiters van bouwwerkinstallaties;

-   (nood)schakelaars van bouwwerkinstallaties.

## Elektrotechniek (discipline)

Alle in het project gerealiseerde bouwdelen binnen deze discipline
worden getekend. Het bestaande wettelijk kader is hiervoor eerste
uitgangspunt. Minimaal gaat het om het tekenen van de volgende bouwdelen
en/of weergave van eigenschappen:

-   brandafsluiters in een E-installatie ter plaatse van een
    compartimentdoorvoer.

## Terrein (discipline)

Alle in het project gerealiseerde bouwdelen binnen deze discipline
worden getekend. Het bestaande wettelijk kader is hiervoor eerste
uitgangspunt.

## Brandveiligheid (aspect)

Alle in het project gerealiseerde brandveiligheidsvoorzieningen worden
getekend. Minimaal gaat het hierbij om de voorzieningen genoemd in NEN
1413:2011

(Beschermde) (sub)brandcompartimenten zijn aangegeven met behulp van
zichtbare en afleesbare compartimentscheidingen die zijn voorzien van
eigenschappen zoals opgenomen in NEN 1413.

Brandveiligheidsvoorzieningen zijn weergegeven met de symbolen zoals
opgenomen in NEN 1413:2011.

Indien brandveiligheidsvoorzieningen hun oorsprong vinden in een andere
discipline (bouwkunde, elektrotechniek, etc.) kan het voorkomen dat een
bouwwerkelement of voorziening meerdere malen gerepresenteerd wordt in
de set revisietekeningen van een bouwwerk. Dit is toegestaan mits de
verschillende representaties onderling niet strijdig zijn.

## Beveiliging (aspect)

Expliciete beveiligingsinformatie wordt opgenomen in aparte
CAD-bestanden. Ook mogen CAD-bestanden in andere disciplines niet
'vervuild’ zijn met expliciete beveiligingsinformatie, anders dan strikt
noodzakelijk voor het doel en de functie van die andere tekeningen.

# Visualisatie

## Basiseisen voor visualisatie

Van elke tekening (aanwezig in de CAD-bestanden behorend tot de
verzameling technisch revisietekenwerk van een project) wordt, naast de
levering van de CAD-bestanden zelf, een visualisatie in
PDF-bestandsformaat geleverd. Deze PDF-bestanden moeten tenminste aan
onderstaande eisen voldoen:

-   bij meer tekeningen in één CAD-bestand worden de resulterende
    PDF-bestanden van elke tekening samenvoegd in één PDF-bestand met
    gelijke naam als het CAD-bestand (exclusief extensie).

-   de getekende en weergegeven onderdelen zijn goed zichtbaar en te
    onderscheiden, ook bij visualisatie van de PDF-bestanden naar papier
    als medium met een afdrukschaal 1:1;

-   de fonts in de PDF-bestanden zijn 'embedded';

-   de PDF-bestanden voldoen aan de PDF standaard;

-   *Layers* aanwezig in een CAD-bestand zijn ook als zodanig aanwezig
    in het bijbehorende PDF-bestand.

## Tekeningformaat

De tekeningen in de *layout tabs* van CAD-bestanden zijn gedefinieerd
als A-formaat volgens NEN 379:2003. Verlenging van A-formaten vindt
plaats volgens NEN 2302:1983 (§ 2.1). Daarnaast is verlenging van een
A4-formaat conform deze methode toegestaan tot een maximaal formaat van
297x1680 mm (8 keer A4 over de lange zijde), toepassing van een verlengd
A0-formaat is toegestaan tot een maximaal formaat van 841x2378 mm (2
keer A0 over de korte zijde).

Alle tekeningen binnen één type projectie binnen één discipline binnen
een project hebben hetzelfde papierformaat[^20].

## Vouwen

Gevisualiseerde tekeningen naar papier als medium worden gevouwen
volgens NEN 2302:1983 (§ 2.2) of NEN 379:2003.

## Lijnen

### Lijnsoorten en lijnsymbolen

Voor de toepassing van lijnsoorten en lijnsymbolen in een tekening is
NEN 2302:1983 van toepassing (§ 4.1).

### Lijndikten

Voor het gebruik van lijndikten in een tekening is § 2.3 van NEN
2302:1983 van toepassing.

### Pentabel

Er worden geen nadere eisen gesteld aan de kleur-pen koppeling.

### Afwijkende ***linetypes***

Alle afwijkende *linetypes* (anders dan getrokken en gestippelde lijnen)
worden verklaard in een renvooi. Indien noodzakelijk voor een goed
begrip van de tekening kan een afwijkend *linetype* voorzien worden van
een verklarende tekst in de tekening in *modelspace*. Verklaring van
afwijkende *linetypes* in een renvooi geldt niet voor:

-   Stramienlijnen.

-   Afbreeklijnen.

-   Componentprojecties.

Het resultaat van visualisatie naar andere media (van de tekening(en)
binnen het CAD-bestand) bevat slechts *linetypes* die goed zichtbaar en
te onderscheiden zijn.

## Arceringen

Voor het gebruik van arceringen in een tekening is NEN 2302:1983 (§ 2.5)
van toepassing. Het resultaat van visualisatie naar andere media (van de
tekening(en) binnen het CAD-bestand) bevat arceerpatronen die goed
zichtbaar en te onderscheiden zijn. Daarnaast zijn de arceerpatronen in
dezelfde bouwdeeldoorsnijdingen en in het daarmee corresponderende
renvooi hetzelfde binnen het technisch revisietekenwerk van één project.

## Schrift

Voor het gebruik van schrift in een tekening is NEN 2302:1983 van
toepassing (§ 2.8). Schrift in de tekeningen moet zijn gesteld in de
Nederlandse taal.

## Schaal

Binnen een tekeningkader in *paperspace* worden entiteiten, getekend in
*modelspace*, zichtbaar gemaakt door middel van één of meerdere
*viewports*. Verschaling van deze entiteiten vindt plaats door middel
van de schaalinstelling gekoppeld aan het desbetreffende *viewport*.
Voor het gebruik van schalen is NEN-ISO 5455:1990 van toepassing. Voor
de verschaling van het te tekenen object (of objecten) binnen een
projectie in een tekening is NEN-ISO 5455:1990 van toepassing.
Tekeningen, gedefinieerd in *paperspace*, zijn bedoeld om afgedrukt te
worden met een plotschaal 1:1 (de gemeten afmetingen in *paperspace*
zijn gelijk aan de gemeten afmetingen op de afgedrukte tekening).

## Oriëntatie

De oriëntatie van het bouwwerk, zowel in het WCS als in de *viewports*
van de tekeningen, is vrij te bepalen. Het heeft echter de voorkeur om
een zodanige oriëntatie te kiezen dat de noordpijl in de tekening naar
de bovenzijde van het tekeningkader wijst. Plattegrondtekeningen worden
voorzien van een noordpijl.

## Ordening van afbeeldingen

Voor de ordening van afbeeldingen in een tekening is NEN 2302:1983 van
toepassing (§ 3.3).

## Symbolische informatie

Voor de visualisatie naar andere media van symbolische informatie in een
tekening is NEN 2302:1983 van toepassing (hoofdstuk 4).

## Maatvoering

### Hoogtematen

Voor het aangeven van hoogtematen in een tekening, is NEN 2302:1983 van
toepassing (§ 5.3.2). Hoogtematen worden gesteld in millimeters.

### Maataanduiding

Voor de visualisatie van maataanduidingen naar andere media in een
tekening is NEN 2302:1983 van toepassing (hoofdstuk 5; inclusief de in
5.1.1 aangegeven voorkeuren).

## Geschreven informatie

Voor geschreven informatie in een tekening is NEN 2302:1983 van
toepassing (hoofdstuk 6).

## Tekeningkader

Elke -binnen een CAD-bestand gedefinieerde- tekening is voorzien van een
tekeningkader. Een tekeningkader bestaat tenminste uit een rechthoek
welke de grenzen van de tekening aangeeft. Naast een rechthoek voor het
aangeven van de grenzen van de tekening bevat een tekeningkader een
markering voor de grenzen van het af te drukken gebied voor visualisatie
naar andere media. De grenzen van het af te drukken gebied voldoen qua
afmetingen aan § . Voor een tekeningkader van een tekening is NEN
2302:1983 van toepassing (§ 2.6). De afstand tussen de grens van de
tekening en de grens van het af te drukken gebied (de 'rand' in § 2.6
van NEN 2302:1983) mag echter kleiner zijn dan de hierin genoemde 20 mm.

## Titelblok

Elke -binnen een CAD-bestand gedefinieerde- tekening is voorzien van een
titelblok. Voor titelblokken is NEN 2302:1983 van toepassing (§ 2.7;
titelblok is identificatiestrook) en NEN-EN-ISO 5457. Bij strijdigheid
van deze normen gaan de eisen in NEN-EN-ISO 5457 boven de eisen in de
NEN 2302:1983.

## Renvooi

Alle, in een tekening voorkomende, arceringen, symbolen en afwijkende
*linetypes* dienen in een renvooi te worden opgenomen met de verklaring
ervan. Een renvooi bestrijkt een verticale strook tussen het titelblok
en de bovenrand van het tekeningkader. Deze strook is niet breder dan
het titelblok.

## Overzichttekening

Wanneer binnen een tekening slechts een onderdeel van een bouwwerk
(bijvoorbeeld een bouwdeel, een ruimte of een detail) afgebeeld wordt
dan wordt er een overzichttekening geplaatst boven het titelblok. Een
overzichttekening moet zodanig worden geplaatst dat deze zichtbaar
blijft op de gevouwen tekening.

De overzichttekening maakt duidelijk waar het desbetreffende onderdeel
van het bouwwerk zich bevindt binnen het totale bouwwerk. Een
overzichttekening bevat bijvoorbeeld de volgende informatie:

-   een schematische situatietekening,

-   een schematische plattegrond van het bouwwerk waarop het totaal en
    het beschouwde deel is aangegeven;

-   een schematische plattegrond van het bouwwerk waarop verdieping en
    kijkrichting is aangegeven.

# Opslag

## Basiseisen voor opslag

Alle op te leveren bestanden (DWG-, PDF- en bronbestanden[^21]) worden
samen met een volledig en correct ingevulde tekeningenlijst opgeleverd
(een XLSX-bestand). Deze tekeningenlijst bevat -van een set bestanden
met technisch revisietekenwerk- per aangeleverde tekening één
registratieregel met in die regel een overzicht van de daarbij horende
kenmerken. In is aangegeven welke tekeningkenmerken uit de
tekeningenlijst moeten corresponderen met een tekeningkenmerk in het
titelblok van een tekening[^22].

Als het RVB bestaand technisch revisietekenwerk ter mutatie aanlevert,
dan worden alle bestanden door de leverancier ook weer opgeleverd, ook
als deze niet zijn gewijzigd. Als het RVB bestaand tekenwerk ter mutatie
aanlevert, dan levert het een tekeningenlijst mee van alle tekeningen en
bestanden in zijn documentbeheeromgeving met betrekking tot de
Bouwwerkcode. Daarin geeft het RVB tevens aan welke bestanden voor
<u>exclusieve</u> mutatie/revisie door de leverancier zijn vrijgegeven
(overige aangeleverde bestanden zijn primair ter informatie en mogelijk
ook al vrijgegeven voor mutatie door andere leveranciers). De
leverancier muteert slechts de bestanden die door het RVB aan de
leverancier worden aangeleverd en zijn vrijgegeven om exclusief door de
leverancier te worden gemuteerd. Als de leverancier het nodig acht ook
andere bestanden te muteren, dan doet zij dit pas nadat zij daarvoor van
de RVB opdrachtgever expliciet toestemming heeft gekregen door middel
van een (aanvullende) vrijgave van die bestanden voor exclusieve
mutatie.

## Mappenstructuur

Bestanden, onderdeel van een set bestanden voor technisch
revisietekenwerk, worden aangeleverd in één map met submappen voor elke
discipline.

## Bestandsnaam

Elk CAD-bestand heeft een unieke bestandsnaam binnen de verzameling
bestandsnamen voor technisch revisietekenwerk van een project. Als het
RVB aan de leverancier geen instructies geeft voor revisie van bestaande
bestanden en/of gebruik van specifieke bestandsnamen, wordt de
bestandsnaam samengesteld uit de volgende bestandskenmerken (zie ook ):

| Bestandskenmerk | Betekenis                                                                                                               | Voorbeeld |
|-----------------|-------------------------------------------------------------------------------------------------------------------------|-----------|
| Bouwwerkcode    | Code waaronder het Bouwwerk in de RVB-systemen geregistreerd is                                                         | 105451G02 |
| Discipline      | Vakdiscipline waaronder de tekening is bewerkt.                                                                         | E         |
| Bouwlaagnummer  | Bouwlaagnummer                                                                                                          | 02        |
| DWG-nummer      | Uniek volgnummer binnen de set bestanden met technisch revisietekenwerk binnen één discipline van één Bouwwerkcode[^23] | 020       |

Syntactisch heeft de naam van het CAD-bestand de volgende opbouw:

\<Bouwwerkcode\>\_\<Discipline\>\_\<Bouwlaagnummer\>\_\<DWG-nummer\>\<.dwg\>

(een voorbeeld van een bestandsnaam is: 105451G02_E\_01_020.dwg).

De PDF-bestandsnamen zijn altijd gelijk aan de naam van het CAD-bestand
waarin één of meerdere tekeningen zijn gedefinieerd, afgezien van de
extensie (elke tekening in het CAD-bestand is een pagina in het
bijbehorende PDF-bestand).

## Bestandsgrootte

Bestanden, onderdeel van een set bestanden voor technisch
revisietekenwerk, zijn niet groter dan 10 Megabyte. In die gevallen waar
deze maximum bestandsgrootte overschreden wordt, of dreigt te worden,
wordt contact opgenomen met de RVB-opdrachtgevervoor overleg over te
nemen maatregelen.

## Titelblok

Elke -binnen een CAD-bestand gedefinieerde- tekening is voorzien van een
titelblok. Binnen een titelblok worden tekeninggebonden kenmerken
vastgelegd. In is aangegeven welke kenmerken uit de tekeningenlijst
moeten corresponderen met een kenmerk in het desbetreffende titelblok.

# Bijlage 1: Definities

## Bouwdeel

Uit materiaal bestaand inwendig element dat invulling geeft aan één of
meer verlangde functies en tevens kan worden onderscheiden naar
materiële samenstelling of constructiewijze.

## Bouwlaag

Deel van een bouwwerk, dat bestaat uit één of meer ruimten, waarbij de
bovenkanten van de afgewerkte vloeren of van het maaiveld van twee aan
elkaar grenzende ruimten niet meer dan 1,5 m in hoogte verschillen.

## Bouwwerk

Een omgevingselement zijnde een constructie van enige omvang van hout,
steen, metaal of ander materiaal, die op de plaats van bestemming hetzij
direct of indirect met de grond verbonden is, hetzij direct of indirect
steun vindt in of op de grond, bedoeld om ter plaatse te functioneren,
met inbegrip van de daarvan deel uitmakende bouwwerkgebonden
installaties.

## Bouwwerkgebonden entiteiten

Entiteiten gedefinieerd in *modelspace* binnen een CAD-bestand, die
direct informatie verschaffen over (onderdelen van) een bouwwerk.
Daarnaast zijn deze entiteiten geen tekeninggebonden entiteiten.

## CAD-bestand

Digitaal bestand aangemaakt door een CAD-programma. CAD staat voor
'Computer Aided Designing/Drafting'. Met CAD-bestand wordt in deze
Specificatie altijd een bestand bedoeld wat technisch revisietekenwerk
bevat en een met AutoCAD bewerkbaar-bestand is zoals omschreven in § .

## Entiteit

AutoCAD-object wat geselecteerd kan worden met één enkele muisklik met
de linkermuisknop.

## Entiteitkenmerk

Eigenschappen van een entiteit.

## *External reference*

Een verwijzing binnen een CAD-bestand naar een ander CAD-bestand. Een
*external reference* wordt zichtbaar binnen een CAD-bestand, maar maakt
daar geen deel van uit. Het bestand waarnaar verwezen wordt, is de
*external reference*. Het bestand waarin een verwijzing naar een
*external reference* is opgenomen, is de *master*.

## Gebouw

Bouwwerk dat betreedbaar en afsluitbaar is.

## Inwendig element

Het kleinste binnen een omgevingselement fysiek herkenbare ruimtelijk
object dat het RVB wenst te onderscheiden.

## Omgevingselement

Het kleinste in de buitenruimte (boven, op of onder het aardoppervlak)
fysiek herkenbare ruimtelijk object dat het RVB wenst te onderscheiden.

## Ruimte

Uit lege ruimte bestaand inwendig element dat voor mensen toegankelijk
is, ten minste aan de onderzijde, en/of de bovenzijde wordt begrensd
door bouwdelen en een netto-hoogte heeft van ten minste 1,5 m.

## Ruimtelijk object

Iets dat een vorm, afmeting en positie heeft ten opzichte van het
aardoppervlak.

## RVB

Afkorting voor het Rijksvastgoedbedrijf, een agentschap van het
ministerie van Binnenlandse Zaken en Koninkrijksrelaties (ministerie
BZK). Als er in deze Specificatie gesproken wordt van aanwijzingen,
bepalingen, materialen of opdrachten die verstrekt worden door het RVB,
dan wordt hiermee het organisatieonderdeel bedoeld dat als opdrachtgever
optreedt voor leveranciers voor de vervaardiging van technisch
revisietekenwerk.

## RVB-object/RVB-gebouw

Een bouwwerk wat als geheel geregistreerd is onder één Bouwwerkcode
binnen de informatiesystemen van het Rijksvastgoedbedrijf. Doorgaans
omvat dit een bouwwerk exclusief het bijbehorende terrein.

## Technisch revisietekenwerk

Technische tekeningen waarop de gerealiseerde situatie ter plaatse wordt
weergegeven, ook wel 'as built'/’as is’/'as maintained' tekenwerk
genoemd.

## Tekening

Het totaal van tekeninggebonden entiteiten en bouwwerkgebonden
entiteiten –welke laatste slechts via de *viewports* zichtbaar zijn in
*paperspace*- en die bedoeld zijn om af te drukken tot een papieren
document ten behoeve van het overdragen van (deel-)informatie over het
bouwwerk. Elke tekening bevat slechts één tekeningkader met daarbinnen
één titelblok.

## Tekeninggebonden entiteiten

Entiteiten gedefinieerd in *paperspace* binnen een CAD-bestand, die
samen een tekening vormen. Het gaat hier om het tekeningkader waarbinnen
het titelblok samen met bijvoorbeeld een renvooi, overzichttekening, een
*viewport* of andere entiteiten geplaatst zijn.

## Titelblok

Het titelblok is een in de tekening opgenomen invulblok dat bedoeld is
ter identificatie van de tekening. Elke tekening bevat slechts één
titelblok. Dit wordt ook wel onderhoek of identificatiestrook genoemd.

NB: Tot 1 april 2010 werd een titelblok volgens RVB model
voorgeschreven. Daarna is het gebruik van een eigen ‘leveranciers’
titelblok voorgeschreven. In is aangegeven welke kenmerken uit de
tekeningenlijst moeten corresponderen met een kenmerk in het
desbetreffende titelblok (zie kolom ‘Zichtbaar in titelblok’).

# Bijlage 2: Tekeningenlijst

Alle aan te leveren bestanden worden altijd samen met een
tekeningenlijst opgeleverd. Deze tekeningenlijst bevat een overzicht van
de te registreren kenmerken (op regel 1)[^24]. Dit bestand bestaat uit
twee tabbladen: 'project en leverancier' en 'tekeningen'. In het tabblad
'project en leverancier' worden project- en leveranciersgegevens
geregistreerd (betrekking hebbend op alle opgeleverde tekeningen samen).
In het tabblad 'tekeningen' worden tekeninggebonden gegevens
geregistreerd: op de regels vanaf regel 2 (de registratieregels) worden
per opgeleverde tekening alle te registreren kenmerken voorzien van een
correcte waarde.

In is per kenmerk een aantal nadere gegevens en eisen vermeld.

-   In kolom 'Kenmerk' wordt een overzicht gegeven van de kenmerken die
    van belang zijn.

-   In de kolom 'Betekenis' wordt nadere uitleg gegeven over de
    kenmerken.

-   In de kolom 'Opgave RVB-opdrachtgever' wordt aangegeven welke
    informatie aangeleverd moet worden door RVB-opdrachtgever bij
    aanleveren van (te muteren) technisch revisietekenwerk aan de
    leverancier.. Deze gegevens mogen niet door een leverancier zelf
    gegenereerd worden en er moeten altijd door de leverancier achteraf
    een of meerdere documenten van de RVB-opdrachtgever getoond kunnen
    worden als bewijs dat deze gegevens zijn aangeleverd.

-   In kolom 'Zichtbaar in titelblok' is aangegeven welke ingevulde
    waarden van kenmerken in de tekeningenlijst ten minste moeten
    corresponderen met informatie in het desbetreffende titelblok van de
    tekeningen.

-   In de kolom 'Opmaak / Toegestane waarden' worden, indien van
    toepassing, specifieke eisen gesteld aan de in te vullen waarde
    onder het desbetreffende kenmerk.

-   In de kolom 'Voorbeeld' wordt een voorbeeld van een ingevulde waarde
    zowel onder het desbetreffende kenmerk in de tekeningenlijst als in
    het titelblok (indien het laatste van toepassing is).

Geef de tekeningenlijst een herkenbare bestandsnaam.

<table>
<colgroup>
<col style="width: 26%" />
<col style="width: 31%" />
<col style="width: 3%" />
<col style="width: 2%" />
<col style="width: 18%" />
<col style="width: 18%" />
</colgroup>
<thead>
<tr class="header">
<th>Kenmerk</th>
<th>Betekenis</th>
<th>Opgave RVB-opdrachtgever</th>
<th>Zichtbaar in titelblok</th>
<th><p>Opmaak /</p>
<p>Toegestane waarden</p></th>
<th>Voorbeeld</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Bouwwerkcode</td>
<td>Code waaronder het Bouwwerk in de RVB-systemen geregistreerd is</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td></td>
<td>105451G02</td>
</tr>
<tr class="even">
<td>Discipline</td>
<td><p>Vakdiscipline waaronder de tekening is bewerkt. Keuze uit:</p>
<p>B=Bouwkunde</p>
<p>C=Constructie<br />
E=Elektrotechniek<br />
T=Terrein<br />
W=Werktuigbouw</p></td>
<td></td>
<td><strong>X</strong></td>
<td>één hoofdletter</td>
<td>B</td>
</tr>
<tr class="odd">
<td>Bouwlaagnummer</td>
<td><p>Locatieaanduiding van tekening in verticale zin. Hier het
Bouwlaagnummer als onderdeel van de Bouwlaagaanduiding:</p>
<p>XX= bouwlaagnummer (oplopend in hoogte)</p>
<p>MB=meerdere bouwlagen</p>
<p>GB=Geen Bouwlaag</p></td>
<td></td>
<td><strong>X</strong></td>
<td>2 posities nummeriek of alfanummeriek</td>
<td>01, 02, 45, MB, GB<a href="#fn1" class="footnote-ref" id="fnref1"
role="doc-noteref"><sup>1</sup></a>,</td>
</tr>
<tr class="even">
<td>DWG-nummer</td>
<td>Uniek volgnummer binnen de set bestanden met technisch
revisietekenwerk binnen één discipline van één Bouwwerkcode</td>
<td></td>
<td></td>
<td>000</td>
<td>020</td>
</tr>
<tr class="odd">
<td>Bestandsnaam</td>
<td>Zie</td>
<td></td>
<td></td>
<td>&lt;Bouwwerkcode&gt;_&lt;Discipline&gt;_&lt;Bouwlaagnummer&gt;_&lt;DWG-nummer&gt;&lt;.dwg&gt;</td>
<td>105451G02_B_01_020.dwg</td>
</tr>
<tr class="even">
<td>Status</td>
<td><p>Status van tekening ten opzichte van door RVB aangeleverde
bronbestanden:</p>
<p>N=nieuwe tekening</p>
<p>G=gewijzigde tekening</p>
<p>O=ongewijzigde tekening</p>
<p>V=vervalt</p></td>
<td></td>
<td></td>
<td>N/G/O/V</td>
<td>G</td>
</tr>
<tr class="odd">
<td>Versie</td>
<td>Versie van de tekening aangeduid met een hoofdletter</td>
<td></td>
<td></td>
<td>één of twee hoofdletters<a href="#fn2" class="footnote-ref"
id="fnref2" role="doc-noteref"><sup>2</sup></a></td>
<td>A, AA</td>
</tr>
<tr class="even">
<td>Vrijgegeven?</td>
<td>Bij aanlevering technisch revisietekenwerk door RVB voor mutatie
door leverancier: vrijgegeven door RVB-opdrachtgever voor exclusieve
mutatie door leverancier</td>
<td><strong>X</strong></td>
<td></td>
<td>JA/NEE</td>
<td></td>
</tr>
<tr class="odd">
<td>Onderwerp-regel1</td>
<td>Hoofdonderwerp; tekstuele beschrijving van het hoofdonderwerp wat de
inhoud van alle tekeningen in één CAD-bestand beschrijft. Inhoud is vrij
te bepalen.</td>
<td></td>
<td><strong>X</strong></td>
<td>Maximaal 100 posities</td>
<td>Gevel, Gevels</td>
</tr>
<tr class="even">
<td>Onderwerp-regel2</td>
<td>Sub onderwerp; tekstuele beschrijving van het sub-onderwerp, de
inhoud van de individuele tekening. Inhoud is vrij te bepalen.</td>
<td></td>
<td><strong>X</strong></td>
<td>Maximaal 100 posities</td>
<td>Noord</td>
</tr>
<tr class="odd">
<td>Gebouwdeel</td>
<td>Locatieaanduiding van tekening in horizontale zin. Optioneel.</td>
<td></td>
<td></td>
<td></td>
<td>Toren C, gebouw A</td>
</tr>
<tr class="even">
<td>Peildatum<a href="#fn3" class="footnote-ref" id="fnref3"
role="doc-noteref"><sup>3</sup></a></td>
<td>Datum van weergegeven toestand m.b.t. bouwwerk<a href="#fn4"
class="footnote-ref" id="fnref4"
role="doc-noteref"><sup>4</sup></a></td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td>DD-MM-JJJJ</td>
<td>12-05-2005</td>
</tr>
<tr class="odd">
<td>Project_nummer</td>
<td>Projectnummer waaronder het project in de RVB-systemen geregistreerd
is</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td></td>
<td><p>60.09254/</p>
<p>10021</p></td>
</tr>
<tr class="even">
<td>Project_naam</td>
<td>Omschrijving van het project</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td></td>
<td>Hoftoren</td>
</tr>
<tr class="odd">
<td>Project_huisadres</td>
<td>Straatnaam + huisnummer van het bouwwerk</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td></td>
<td>Kostverlorenkade 23</td>
</tr>
<tr class="even">
<td>Project_postcode</td>
<td>Postcode van het bouwwerk</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td>0000 XX</td>
<td>2511 VE</td>
</tr>
<tr class="odd">
<td>Project_plaats</td>
<td>Plaats van het bouwwerk</td>
<td><strong>X</strong></td>
<td><strong>X</strong></td>
<td></td>
<td>Den Haag</td>
</tr>
<tr class="even">
<td>Leverancier_bedrijfsnaam</td>
<td>Bedrijfsnaam van de leverancier van de volledige opgeleverde set
technisch revisietekenwerk</td>
<td></td>
<td><strong>X</strong></td>
<td></td>
<td>Allbouw BV</td>
</tr>
<tr class="odd">
<td>Leverancier_postadres</td>
<td>Postbus + nummer / straatnaam + huisnummer van het postadres</td>
<td></td>
<td></td>
<td></td>
<td>Postbus 201 / Bouwwerkweg 3</td>
</tr>
<tr class="even">
<td>Leverancier_postcode</td>
<td>Postcode van het postadres</td>
<td></td>
<td></td>
<td>0000 XX</td>
<td>1234 AA</td>
</tr>
<tr class="odd">
<td>Leverancier_plaats</td>
<td>Plaatsnaam van het postadres</td>
<td></td>
<td></td>
<td></td>
<td>Werkstad</td>
</tr>
<tr class="even">
<td>Leverancier_contactpersoon</td>
<td>Naam contactpersoon leverancier</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>Leverancier_telefoon</td>
<td>Telefoonnummer contactpersoon leverancier</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>Leverancier_e-mailadres</td>
<td>E-mailadres contactpersoon leverancier</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>
<section class="footnotes footnotes-end-of-document"
role="doc-endnotes">
<hr />
<ol>
<li id="fn1" role="doc-endnote"><p>Geen bouwlaag.<a href="#fnref1"
class="footnote-back" role="doc-backlink">↩︎</a></p></li>
<li id="fn2" role="doc-endnote"><p>Als alle letters van het alfabet
gebruikt zijn, dan worden dubbele hoofdletters AA, BB, CC enzovoort
gebruikt.<a href="#fnref2" class="footnote-back"
role="doc-backlink">↩︎</a></p></li>
<li id="fn3" role="doc-endnote"><p>Van belang is hier dat de
RVB-opdrachtgever -in overleg met alle leveranciers van
revisietekenwerk- een datum vaststelt voor de weer te geven toestand met
betrekking tot alle bij het project betrokken disciplines. Veelal zal
dit een datum zijn waarop het RVB-object na oplevering 'in rust' is,
bijvoorbeeld de datum van de tweede oplevering.<a href="#fnref3"
class="footnote-back" role="doc-backlink">↩︎</a></p></li>
<li id="fn4" role="doc-endnote"><p>Het gaat hier dus niet om de
aanmaakdatum (is datum aanmaak van een tekening) of de revisiedatum (is
datum dat de tekening voor het laatst is bijgewerkt). Alleen de datum
van de weergegeven toestand is hier voor het RVB van belang.<a
href="#fnref4" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
</ol>
</section>

Tabel 2: kenmerken in de tekeningenlijst en/of het titelblok

# Bijlage 3: Normenoverzicht

-   Bond van Nederlandse Architecten (BNA): NL/SfB tabellen 2005
    inclusief herziene Elementenmethode ’91; Amsterdam; ISBN-10:
    90-807626-3-6

-   NEN-ISO 128-40:2001: Technische tekeningen - Algemene principes voor
    de weergave - Deel 40: Basisafspraken voor doorsneden

    -   de bepalingen onder NEN-ISO 128-50:2001 § 9 zijn niet van
        toepassing

-   NEN-ISO 5455:1990 & /C1:1996: Technische tekeningen. Schalen

-   NEN-ISO 5456-1:1997: Technisch tekenen. Projectiemethoden. Deel 1:
    Overzicht

-   NEN-ISO 5456-2:1997: Technisch tekenen. Projectiemethoden. Deel 2:
    Orthografische afbeeldingen

-   NEN-EN-ISO 5457:1999 & /A1:2010: Technische product-documentatie --
    Formaten en inrichting van tekenbladen

    -   inclusief de in § 3.1 genoemde voorkeuren

    -   de bepalingen onder § 4.3, § 4.4, § 4.5 zijn optioneel

    -   de bepalingen onder NEN-EN-ISO 7200:2004 § 5 zijn optioneel

-   NEN 1413:2011 : Symbolen voor veiligheidsvoorzieningen op
    bouwkundige tekeningen en in bouwkundige schema’s

-   NEN 2302:1983: Tekeningen in de bouw -- Algemene regels

    -   de bepalingen onder § 2.7.1 zijn optioneel

    -   inclusief de in § 5.1.1 genoemde voorkeuren

-   NEN 2574:1993 Tekeningen in de bouw - Indeling van gegevens op
    tekeningen voor gebouwen

-   NPR 2570:1986: Tekeningen in de bouw -- Coördinatie van gegevens op
    tekeningen voor gebouwen

    -   uitsluitend § 2

-   NEN 379:2003: Technische productdocumentatie - Vouwen en inhechten
    van tekenbladen

[^1]: Deze CAD Specificatie vervangt de Norm voor technisch
    revisietekenwerk'

[^2]: AutoCAD is een geregistreerd handelsproduct van Autodesk
    Incorporated.

[^3]: AutoCAD-termen worden in deze Specificatie cursief weergegeven.

[^4]: Een gerasterd bedrijfslogo in het titelblok is toegestaan.

[^5]: Voor hoogwaardig technisch revisietekenwerk waarvoor *ObjectARX*
    entiteiten van grote waarde is kan het zinnig zijn deze *ObjectARX*
    entiteiten te behouden. In deze gevallen beslist de
    RVB-opdrachtgever over de wijze van aanlevering.

[^6]: Met CAD-bestand wordt in deze Specificatie altijd een bestand
    bedoeld wat technisch revisietekenwerk bevat en een AutoCAD-bestand
    is zoals omschreven in § .

[^7]: Voor hoogwaardig technisch revisietekenwerk waarvoor database
    koppelingen van grote waarde is kan het zinnig zijn deze database
    koppelingen te behouden. In deze gevallen beslist de
    RVB-opdrachtgever over de wijze van aanlevering.

[^8]: In sommige andere normen ook wel 'doorsnijdingsvlak' genoemd.

[^9]: Als daarmee een tekening ontstaat die niet goed afleesbaar is en
    tot ongewenste bouwkundige interpretaties aanleiding geeft, dan mag
    het projectievlak op een andere hoogte gelegd worden (ook lokaal).
    In deze gevallen wordt in de tekening een toelichtende tekst
    toegevoegd.

[^10]: Waar is deze Specificatie het begrip 'bouwwerk' gebruikt wordt,
    wordt het begrip 'omgevingselement' bedoeld. Zie Bijlage 1:
    Definities voor de betekenis van en het onderscheid tussen deze
    begrippen.

[^11]: Met dit laatste wordt bedoeld dat als er in een doorsnede een
    gevel wordt weergegeven (in het projectievlak wordt ook een gevel
    van het werk geprojecteerd), deze gevel moet worden getekend volgens
    de eisen die er aan gevels worden gesteld in deze Specificatie.

[^12]: Met dit laatste wordt bedoeld dat als er in een gevel een
    doorsnede wordt weergegeven (het projectievlak doorsnijdt ook het
    werk zelf), deze doorsnede moet worden getekend volgens de eisen die
    er aan doorsneden worden gesteld in deze Specificatie.

[^13]: Uitgave van de Bond van Nederlandse Architecten, Amsterdam;
    ISBN-10: 90-807626-3-6

[^14]: Het hoofdonderwerp is de belangrijkste zoeksleutel binnen een
    discipline. De beschrijving hiervan moet specifiek genoeg zijn.
    Bijvoorbeeld: ‘elektrotechnische installatie’ is te generiek en
    wordt al aangegeven door de letter van de discipline. Woorden als
    'definitief', 'nieuw', 'diverse' of 'revisie' zijn niet toegestaan.
    Goede voorbeelden zijn: Plattegrond, Gevels, Doorsneden,
    Lichtinstallatie, Terreininstallatie, Veiligheidsvoorzieningen, CV-
    en ventilatie-installatie.

[^15]: Binnen AutoCAD bestaan er twee typen *external reference*:
    *overlay* en *attached*. Het verschil tussen deze twee types is het
    gedrag bij meervoudige innesteling. In tegenstelling tot het *Xref*
    type *attached* wordt een *external reference* van het type
    *overlay* niet ‘meegenomen’ wanneer het bestand met de betreffende
    *Xref* verwijzingen op zijn beurt weer d.m.v. *Xref* wordt gekoppeld
    wordt aan een volgend bestand.

[^16]: Voor vloeren is dit de bovenzijde van de afgewerkte vloer.

[^17]: Uitgave van de Bond van Nederlandse Architecten, Amsterdam;
    ISBN-10: 90-807626-3-6

[^18]: Als het project uitgevoerd wordt op basis van Output
    Specificaties, zoals door het RVB in bepaalde contractsvormen
    gehanteerd, dan wordt hier de ‘OS functienaam 2D’ voor gebruikt. In
    deze context wordt met functienaam de naam bedoeld van een
    individueel ruimtetype (functie) in de ‘ruimteboom’ van de Output
    Specificatie.

[^19]: Uitgave van de Bond van Nederlandse Architecten, Amsterdam;
    ISBN-10: 90-807626-3-6

[^20]: Belangrijk is dat er bij naastliggende deeltekeningen slechts
    beperkte overlap zit in het deel wat in de ene tekening wordt
    weergegeven en het deel wat in de andere –naastliggende- tekening
    wordt weergegeven.

[^21]: Zie §

[^22]: Een lege tekeninglijst met daarin een overzicht van de te
    registreren kenmerken is verkrijgbaar op de website van het
    Rijksvastgoedbedrijf samen met deze Specificatie (versie nummer van
    de tekeninglijst correspondeert met het versie nummer van de
    Specificatie). Deze tekeninglijst wordt gebruikt voor importeren van
    de aangeleverde bestanden met de metadata in de
    documentbeheeromgeving van het Rijksvastgoedbedrijf. Gebruik en
    levering van andere tekeningenlijsten is niet toegestaan.

[^23]: Bij aanleveren van revisietekenwerk door het RVB levert het RVB
    een tekeninglijst mee van alle bestanden/tekeningen technisch
    revisietekenwerk onder de Bouwwerkcode in zijn
    documentbeheeromgeving. Bij aanmaak van nieuwe bestanden binnen een
    bestaande set revisietekenwerk bestanden zorgt de leverancier aan de
    hand van deze lijst voor unieke DWG-nummers in deze nieuwe
    bestandsnamen.

[^24]: Een lege tekeninglijst met daarin een overzicht van de te
    registreren kenmerken is verkrijgbaar op de website van het RVB
    samen met deze Specificatie.
