<img src="media/image1.jpg" style="width:8.25in;height:11.66333in" />

# Voorwoord 

Het Rijksvastgoedbedrijf is de vastgoedorganisatie van en voor de
Rijksoverheid. Het

Rijksvastgoedbedrijf is verantwoordelijk voor instandhouding en beheer
van de grootste en meest diverse vastgoedportefeuille van Nederland. Het
Rijksvastgoedbedrijf treedt vanuit zijn rol veelal op als
eindopdrachtgever. Voor een adequaat beheer van de portefeuille is
actuele vastgoedinformatie noodzakelijk. Vastgoedinformatie wordt vaak
vastgelegd in tekeningen, naast andere wijzen van vastlegging. Bij
nieuwbouw, verbouw, aankoop, aanhuur en onderhoud van bouwwerken worden
tekeningen geraadpleegd en vervaardigd. Vooral tekeningen waarop de
gerealiseerde situatie ter plaatse wordt weergegeven -technisch
revisietekenwerk of 'as built'/’as is’/'as maintained' tekenwerk- zijn
voor het Rijksvastgoedbedrijf van belang. Het Rijksvastgoedbedrijf stelt
met deze CAD Specificatie[1] eisen aan dit technisch revisietekenwerk.

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

**Leeswijzer**

<img src="media/image2.png" style="width:3.08472in;height:2.91944in" />Technisch
revisietekenwerk wordt geleverd in een CAD-bestand. CAD-bestanden zijn
te beschrijven in vier dimensies: structuur, inhoud, visualisatie en
opslag. Bij structuur gaat het om de samenhang, en daarmee de betekenis,
van de entiteiten aangebracht binnen een CAD-bestand. Bij inhoud gaat
het om het vastleggen van de werkelijkheid met behulp van deze
gestructureerde en betekenisvolle entiteiten. Bij visualisatie gaat het
om de vertaling van de aangebrachte inhoud en structuur in een
CAD-bestand naar een ander medium voor ter beschikkingstelling van de
informatie. Bij opslag gaat het om de opslag van een CAD-bestand. Voor
elke dimensie zijn er in deze Specificatie eisen opgesteld.

De hoofdstukken 1 tot en met 4 beschrijven de eisen voor technisch
revisietekenwerk met betrekking tot deze vier dimensies. In de bijlagen
komen achtereenvolgend definities, tekeningenlijst en normenoverzicht
aan bod.

# Inhoudsopgave 

[Voorwoord 3](#voorwoord)

[Inhoudsopgave 4](#inhoudsopgave)

[1 Structuur 6](#structuur)

[1.1 CAD-bestanden 6](#cad-bestanden)

[1.1.1 Bestandsformaat 6](#bestandsformaat)

[1.1.2 Database koppelingen 6](#database-koppelingen)

[1.1.3 Systeemvariabelen 6](#systeemvariabelen)

[1.2 Levering bronbestanden 6](#levering-bronbestanden)

[1.3 Basisprincipes voor technisch revisietekenwerk
7](#basisprincipes-voor-technisch-revisietekenwerk)

[1.3.1 Projectievlak 7](#projectievlak)

[1.3.2 Plattegronden 11](#plattegronden)

[1.3.3 Doorsneden 11](#doorsneden)

[1.3.4 Gevels 11](#gevels)

[1.3.5 Entiteiten getekend in het *WCS*
11](#entiteiten-getekend-in-het-wcs)

[1.4 Informatiescheiding met behulp van *layers*
11](#informatiescheiding-met-behulp-van-layers)

[1.5 *Layout tabs* 12](#layout-tabs)

[1.5.1 Gebruik van *layout tabs* 12](#gebruik-van-layout-tabs)

[1.5.2 Naamgeving van *layout tabs* 12](#naamgeving-van-layout-tabs)

[1.6 *Paperspace* 12](#paperspace)

[1.6.1 Tekeningkader en titelblok 12](#tekeningkader-en-titelblok)

[1.6.2 Gebruik van *blocks* 12](#gebruik-van-blocks)

[*1.6.3* Naamgeving van *blocks* 12](#naamgeving-van-blocks)

[1.6.4 Gebruik van *external references*
12](#gebruik-van-external-references)

[1.6.5 Tekeninggebonden tekst 13](#tekeninggebonden-tekst)

[1.7 *Modelspace* 13](#modelspace)

[1.7.1 Gebruik van *blocks* 13](#gebruik-van-blocks-1)

[*1.7.2* Naamgeving van *blocks* 13](#naamgeving-van-blocks-1)

[1.7.3 Gebruik van *external references*
13](#gebruik-van-external-references-1)

[1.7.4 Positie bouwwerk 13](#positie-bouwwerk)

[1.7.5 Stramien 13](#stramien)

[1.7.6 Hoogtematen 13](#hoogtematen)

[1.7.7 Maataanduiding 13](#maataanduiding)

[1.7.8 Bouwwerkgebonden tekst 13](#bouwwerkgebonden-tekst)

[1.8 Tekeningsoort 13](#tekeningsoort)

[1.9 Detailleringniveau 14](#detailleringniveau)

[1.10 Nauwkeurigheid 14](#nauwkeurigheid)

[1.11 Bouwlaagaanduiding 14](#bouwlaagaanduiding)

[1.12 Constructie (discipline) 14](#constructie-discipline)

[1.13 Bouwkunde (discipline) 14](#bouwkunde-discipline)

[1.14 Werktuigbouw (discipline) 14](#werktuigbouw-discipline)

[1.15 Elektrotechniek (discipline) 14](#elektrotechniek-discipline)

[1.16 Terrein (discipline) 15](#terrein-discipline)

[1.17 Brandveiligheid (aspect) 15](#brandveiligheid-aspect)

[1.18 Beveiliging (aspect) 15](#beveiliging-aspect)

[2 Inhoud 16](#inhoud)

[2.1 Basiseisen voor inhoud 16](#basiseisen-voor-inhoud)

[2.2 Constructie (discipline) 16](#constructie-discipline-1)

[2.3 Bouwkunde (discipline) 17](#bouwkunde-discipline-1)

[2.3.1 Basis bouwdeelniveau Bouwkunde
17](#basis-bouwdeelniveau-bouwkunde)

[2.3.2 Stramien 17](#stramien-1)

[2.3.3 Hoogtematen 17](#hoogtematen-1)

[2.3.4 Maataanduiding 17](#maataanduiding-1)

[2.3.5 Ruimtenaam 17](#ruimtenaam)

[2.3.6 Ruimtecode 17](#ruimtecode)

[2.4 Werktuigbouw (discipline) 17](#werktuigbouw-discipline-1)

[2.5 Elektrotechniek (discipline) 18](#elektrotechniek-discipline-1)

[2.6 Terrein (discipline) 18](#terrein-discipline-1)

[2.7 Brandveiligheid (aspect) 18](#brandveiligheid-aspect-1)

[2.8 Beveiliging (aspect) 18](#beveiliging-aspect-1)

[3 Visualisatie 19](#visualisatie)

[3.1 Basiseisen voor visualisatie 19](#basiseisen-voor-visualisatie)

[3.2 Tekeningformaat 19](#tekeningformaat)

[3.3 Vouwen 19](#vouwen)

[3.4 Lijnen 19](#lijnen)

[3.4.1 Lijnsoorten en lijnsymbolen 19](#lijnsoorten-en-lijnsymbolen)

[3.4.2 Lijndikten 19](#lijndikten)

[3.4.3 Pentabel 19](#pentabel)

[3.4.4 Afwijkende *linetypes* 19](#afwijkende-linetypes)

[3.5 Arceringen 20](#arceringen)

[3.6 Schrift 20](#schrift)

[3.7 Schaal 20](#schaal)

[3.8 Oriëntatie 20](#oriëntatie)

[3.9 Ordening van afbeeldingen 20](#ordening-van-afbeeldingen)

[3.10 Symbolische informatie 20](#symbolische-informatie)

[3.11 Maatvoering 20](#maatvoering)

[3.11.1 Hoogtematen 20](#hoogtematen-2)

[3.11.2 Maataanduiding 20](#maataanduiding-2)

[3.12 Geschreven informatie 20](#geschreven-informatie)

[3.13 Tekeningkader 21](#tekeningkader)

[3.14 Titelblok 21](#titelblok)

[3.15 Renvooi 21](#renvooi)

[3.16 Overzichttekening 21](#overzichttekening)

[4 Opslag 22](#opslag)

[4.1 Basiseisen voor opslag 22](#basiseisen-voor-opslag)

[4.2 Mappenstructuur 22](#mappenstructuur)

[4.3 Bestandsnaam 23](#bestandsnaam)

[4.4 Bestandsgrootte 23](#bestandsgrootte)

[4.5 Titelblok 23](#titelblok-1)

[Bijlage 1: Definities 24](#bijlage-1-definities)

[Bouwdeel 24](#bouwdeel)

[Bouwlaag 24](#bouwlaag)

[Bouwwerk 24](#bouwwerk)

[Bouwwerkgebonden entiteiten 24](#bouwwerkgebonden-entiteiten)

[CAD-bestand 24](#cad-bestand)

[Entiteit 24](#entiteit)

[Entiteitkenmerk 24](#entiteitkenmerk)

[*External reference* 24](#external-reference)

[Gebouw 24](#gebouw)

[Inwendig element 25](#inwendig-element)

[Omgevingselement 25](#omgevingselement)

[Ruimte 25](#ruimte)

[Ruimtelijk object 25](#ruimtelijk-object)

[RVB 25](#rvb)

[RVB-object/RVB-gebouw 25](#rvb-objectrvb-gebouw)

[Technisch revisietekenwerk 25](#technisch-revisietekenwerk)

[Tekening 25](#tekening)

[Tekeninggebonden entiteiten 25](#tekeninggebonden-entiteiten)

[Titelblok 25](#titelblok-2)

[Bijlage 2: Tekeningenlijst 26](#bijlage-2-tekeningenlijst)

[Bijlage 3: Normenoverzicht 29](#bijlage-3-normenoverzicht)

