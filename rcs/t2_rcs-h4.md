# Opslag 

## Basiseisen voor opslag 

Alle op te leveren bestanden (DWG-, PDF- en bronbestanden[21]) worden
samen met een volledig en correct ingevulde tekeningenlijst opgeleverd
(een XLSX-bestand). Deze tekeningenlijst bevat -van een set bestanden
met technisch revisietekenwerk- per aangeleverde tekening één
registratieregel met in die regel een overzicht van de daarbij horende
kenmerken. In Bijlage 2: Tekeningenlijst is aangegeven welke
tekeningkenmerken uit de tekeningenlijst moeten corresponderen met een
tekeningkenmerk in het titelblok van een tekening[22].

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
bestandsnaam samengesteld uit de volgende bestandskenmerken (zie ook
Bijlage 2: Tekeningenlijst):

<table>
<colgroup>
<col style="width: 25%" />
<col style="width: 59%" />
<col style="width: 15%" />
</colgroup>
<thead>
<tr class="header">
<th><blockquote>
<p><em><strong>Bestandskenmerk</strong></em></p>
</blockquote></th>
<th><blockquote>
<p><em><strong>Betekenis</strong></em></p>
</blockquote></th>
<th><blockquote>
<p><em><strong>Voorbeeld</strong></em></p>
</blockquote></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>Bouwwerkcode</p>
</blockquote></td>
<td><blockquote>
<p>Code waaronder het Bouwwerk in de RVBsystemen geregistreerd is</p>
</blockquote></td>
<td><blockquote>
<p>105451G02</p>
</blockquote></td>
</tr>
<tr class="even">
<td><blockquote>
<p>Discipline</p>
</blockquote></td>
<td><blockquote>
<p>Vakdiscipline waaronder de tekening is bewerkt.</p>
</blockquote></td>
<td>E</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>Bouwlaagnummer</p>
</blockquote></td>
<td><blockquote>
<p>Bouwlaagnummer</p>
</blockquote></td>
<td><blockquote>
<p>02</p>
</blockquote></td>
</tr>
<tr class="even">
<td><blockquote>
<p>DWG-nummer</p>
</blockquote></td>
<td><blockquote>
<p>Uniek volgnummer binnen de set bestanden met technisch revisietekenwerk binnen één discipline van één Bouwwerkcode<a href="#fn1" class="footnote-ref" id="fnref1" role="doc-noteref"><sup>1</sup></a></p>
</blockquote></td>
<td><blockquote>
<p>020</p>
</blockquote></td>
</tr>
</tbody>
</table>
<section class="footnotes" role="doc-endnotes">
<hr />
<ol>
<li id="fn1" role="doc-endnote"><p>Bij aanleveren van revisietekenwerk door het RVB levert het RVB een tekeninglijst mee van alle bestanden/tekeningen technisch revisietekenwerk onder de Bouwwerkcode in zijn documentbeheeromgeving. Bij aanmaak van nieuwe bestanden binnen een bestaande set revisietekenwerk bestanden zorgt de leverancier aan de hand van deze lijst voor unieke DWG-nummers in deze nieuwe bestandsnamen.<a href="#fnref1" class="footnote-back" role="doc-backlink">↩︎</a></p></li>
</ol>
</section>

Syntactisch heeft de naam van het CAD-bestand de volgende opbouw:

#### \<Bouwwerkcode>\_\<Discipline>\_\<Bouwlaagnummer>\_\<DWG-nummer>\<.dwg> 

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
vastgelegd. In Bijlage 2: Tekeningenlijst is aangegeven welke kenmerken
uit de tekeningenlijst moeten corresponderen met een kenmerk in het
desbetreffende titelblok.

