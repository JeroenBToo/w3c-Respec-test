# Structuur

## CAD-bestanden

### Bestandsformaat

Technisch revisietekenwerk wordt geleverd in een bestandsformaat dat geopend, bewerkt en opgeslagen kan worden met het programma AutoCAD2: het dwg-bestandsformaat(dwg-formaat). Bij deze handelingen in dit softwarepakket mag er geen foutmelding optreden of informatie verloren gaan. Afzonderlijk herkenbare entiteiten zijn in dit bestand ook als zodanig gedefinieerd en door dit softwarepakket herkenbaar,zonder dat daar extra verticale applicaties op zijn geïnstalleerd(bijvoorbeeld: tekst is text,3lijnen zijn linesof polylines, arceringen zijn hatches, maatvoeringen zijn dimensionsen cirkels zijn circles). Verder voldoen de bestanden aan de volgende voorwaarden:
* de bestanden zijnaltijd gebaseerd op een metrisch template;
* de bestanden zijn niet beveiligd door gebruik te maken van enige vorm van encryptie;
* de bestanden bevatten geen ‘OLE-objecten’;
* de bestanden bevatten geen dictionaries, behalve die door AutoCADzélfautomatisch worden gegenereerd;
* de bestanden bevatten geen gerasterde entiteiten4;
* de bestanden bevatten geen, in het bestand geïntegreerde, LISP-of VBA-routines;
* de bestanden bevatten geen entiteiten waaraan ‘hyperlinks’ gekoppeld zijn;
* de bestanden bevatten geen entiteiten gegenereerd en ondersteund door ObjectARX-applicaties5(of: proxy-objecten), anders dandoor AutoCADzèlf automatisch gegenereerde(informatie over deze ‘add-ons’ isniet aanwezigende samengestelde objecten zijncorrectvertaald naar AutoCAD-basisentiteitenende koppeling naar de gebruikte ‘add-on’ isverbroken).

### Database koppelingen

De CAD-bestanden6voor technisch revisietekenwerk bevatten geen koppelingen naar externe databases7. Alle restinformatie binnen deze CAD-bestanden, als gevolg van dergelijke 'database-connectivity' uit het verleden, is niet meer aanwezig.

### Systeemvariabelen

Binnen elk CAD-bestand zijn er system variablesvastgelegd. Deze systeemvariabelen zijn van invloed op diverse onderdelen binnen deze bestanden. De systeemvariabelen hebben de waarden volgens de onderstaande tabel.

| VARIABELE | WAARDE |
|---|---|
| LUNITS | 2 |
| LWDISPLAY | OFF |
| MEASUREMENT | 1 |

## Levering bronbestanden
