# Metadata

Introductie metadata

## INSPIRE-metadata in het Nationaal Georegister
In het figuur hieronder zie je een screenshot van het Nationaal Georegister (NGR), dat voor INSPIRE-metadata dienst doet als *discovery service*. Het NGR wordt echter niet alleen met INSPIRE-conforme metadata gevuld; ook andere metadata kan toegevoegd worden. INSPIRE-metadata kan gevonden worden door in het tabblad 'Zoeken' te filteren op de Categorie 'Inspire'.

![NGRinspire](media/NGR-FilterINSPIRE.png "Gebruik in het NGR het filter 'Inspire' om alle beschikbare INSPIRE-compliant datasets te vinden.")

## Metadata aanmaken
Metadata dient ter beschikking worden gesteld voor:
- Datasets en dataset series, én;
- Network Services (o.a. View en Download Services).

Normaal gesproken zal de dataprovider metadata aanmaken als onderdeel van beheer en publicatie van data en services. De dataprovider heeft daarbij ook de taak om na te gaan of deze metadatabestanden (XML-bestanden) voldoen aan de INSPIRE-richtlijnen. De via deze weg aangemaakte metadata wordt vervolgens in het Nationaal Georegister (NGR) gepubliceerd door het uploaden van XML-metadatabestanden, of door harvesting vanuit een eigen metadatacatalogus.

Het aanmaken en publiceren van metadata kan ook rechtstreeks via het Nationaal Georegister. Binnen het NGR is hiervoor een metadata-editor beschikbaar.

## Eisen metadata
De metadata-elementen die voor INSPIRE, vanuit verschillende richtlijnen, beschreven moeten worden zijn opgenomen in de Nederlandse profielen. Deze profielen zijn conform de INSPIRE-richtlijn. In de profielen zijn verplichte en door conditie verplichte elementen opgenomen. Om te voldoen aan de INSPIRE-vereisten, moeten de conditionele elementen voor INSPIRE ook worden beschreven en aan de condities voor INSPIRE voldoen.

Zie voor meer informatie het [dossier metadata op de Geonovum-website](https://www.geonovum.nl/geo-standaarden/metadata).

## Metadata en taal
In de invoeringsregels voor metadata is niets vastgelegd over de taal waarin metadata beschikbaar moet worden gesteld. Wél worden de in de bron (dataset en service) gebruikte taal en de metadata-taal vastgelegd. In de [*Technical Guidance*](https://inspire.ec.europa.eu/id/document/tg/metadata-iso19139) staat beschreven hoe vrije tekstvelden in meerdere talen kunnen worden opgenomen.

INSPIRE laat open in welke taal de metadata wordt ingevoerd. Nederland hefet ervoor gekozen om de metadata in het Nederlands op te voeren, waarbij 'dut' de waarde van de metadata-taal is. Als er aanvullend voor een extra taal wordt gekozen, dient deze consequent gehanteerd te worden. Stelt u bijvoorbeeld de metadata ook in het Engels beschikbaar, dan dienen alle vrije tekstvelden in de metadata vertaald te worden. Denk daarbij ook aan de licentie zelf.

De *Get Network Service Metadata*-respons van de netwerkdienst (de view- en downloadservice) moet alle metadata-elementen bevatten die zijn opgenomen in de ISO 19139-metadata in alle ondersteunde talen in die service.

De services zijn mono-linguïstisch, voor elke ondersteunde taal zal er een ander document moeten zijn. Alle gerelateerde INSPIRE-servicesdocumenten, zoals de tekst in de dataset, de legendatekst, de capability-documenten en de foutmeldingen, zullen eveneens in het Engels beschikbaar moeten zijn.

In de metadata werkt het anders en kan middels extra elementen vertalingen van alle string-elementen worden toegevoegd.

Als er met meertaligheid wordt gewerkt, hou dan rekening met het volgende:
- De metadata-taal is dezelfde als de default-taal van de services, in ons geval Nederlands.
- Als je de metadata gaat vertalen zal dat voor alle vrijetekst-elementen moeten gebeuren. Denk daarbij ook aan de licenties van toegangsrestricties etc.
- Voor elke ondersteunde taal in de service, moet ook een vertaling in de metadata aanwezig zijn.
- Voor elke ondersteunde taal in de service, zijn aparte capabilities-, legenda- en foutmeldingsdocumenten nodig.

## Geharmoniseerde gebruiksvoorwaarden
De gebruiksvoorwaarden worden opgenomen in de metadata. Wie geo-informatie van een ander gebruikt, moet weten of daarvoor voorwaarden gelden en zo ja, welke voorwaarden dat zijn. De Nederlandse overheid wil overheidsinformatie zoveel mogelijk gratis en zonder gebruiksvoorwaarden beschikbaar stellen. Dat kan met behulp van de **Public Domain Mark** of met de **Creative Commons Zero (CC0)**-verklaring. Met beide gebruiksvoorwaarden zijn de gegevens door iedereen voor ieder doeleind te gebruiken. Het verschil is dat op gegevens met een CC0-verklaring een auteurs-, databank- of ander recht van kracht is. Met de CC0-verklaring wordt afstand gedaan van deze rechten. Het ministerie van BZK hanteert Creative Commons Zero als de voorkeurslicentie voor data van haar ministerie.

### Public Domain Mark
Gegevens die met de Public Domain Mark beschikbaar zijn gesteld, kunnen door iedereen voor alle doeleinden worden gebruikt. Ook naamsvermelding kan niet geëist worden. U vindt de tekst die bij de Public Domain Mark hoort op de [site van Creative Commons](https://creativecommons.org/publicdomain/mark/1.0/deed.nl).

### Creative Commons Zero
Als er auteursrecht en/of databankenrecht rust op gegevens, of als bij wet, besluit of verordening het openbaarmaken van gegevens uitdrukkelijk is voorbehouden, is de Public Domain Mark niet mogelijk. Om ook in dit geval gegevens zonder verdere vereisten beschikbaar te stellen, kan de Creative Commons Zero-verklaring worden gebruikt. Met deze verklaring geeft de eigenaar aan de geldende rechten niet te zullen uitoefenen. U vindt de tekst die bij de Creative Commons Zero-verklaring hoort op de [site van Creative Commons](https://creativecommons.org/publicdomain/zero/1.0/deed.nl).

### Gebruiksvoorwaarden in Nederland
In Nederland is afgesproken om voor geo-informatie gebruik te maken van de gebruiksvoorwaarden van Creative Commons, tenzij dat niet mogelijk is. Dit “Creative Commons, tenzij”-beleid is in 2014 vastgesteld door het GI-beraad. [Deze tool](https://creativecommons.org/choose/?lang=nl) kan gebruikt worden om een CC-licentie samen te stellen.

In sommige gevallen is het toch noodzakelijk om gebruiksvoorwaarden te handhaven, bijvoorbeeld door wetgeving. In die gevallen biedt Geo Gedeeld uitkomst. Geo Gedeeld is een hulpmiddel om gebruiksvoorwaarden voor geo-informatie op een eenvoudige, heldere en gestandaardiseerde manier kenbaar te maken. Het is ontstaan uit de behoefte van de overheid om de bestaande gebruiksvoorwaarden voor geo-informatie te stroomlijnen. [Deze website](http://geogedeeld.geonovum.nl/) kan gebruikt worden om een GG-licentie samen te stellen.

De gebruiksvoorwaarden, ook als daarvan wordt afgezien in Public Domain Mark of Creative Commons Zero-verklaring, worden opgenomen in de metadata. De instructie hiervoor is te vinden in de paragraaf [Invulinstructies voor datasets](#invulinstructies-voor-datasets).

## Invulinstructies voor datasets
De onderstaande tabel geeft invulinstructies die van belang zijn bij INSPIRE-metadata-elementen. Let erop, dat er zowel verplichte ('Ja') als conditionele ('C') elementen in voorkomen. Zo kan bijvoorbeeld een aantal elementen pas worden ingevuld wanneer de dataharmonisatie is voltooid. Voor prioritaire datasets is de [aanvullende instructie](#prioritaire-datasets) over het opnemen van de trefwoorden in de metadata nu ook in de invulinstructies meegenomen.


| Metadata-element 									| Longname 		| INSPIRE-verplicht | Omschrijving 	| Voorbeeldwaarde |
|------------										|-------------	|-------------		|------------	|-------|
| **URL**  											| MD_Metadata.distributionInfo> MD_Distribution.transferOptions> MD_DigitalTransferOptions.onLine> CI_OnlineResource.linkage | Ja | Voor INSPIRE wordt hier ten minste de URL van de view- en de downloadservice opgenomen. Als er meerdere datasets in één service worden ontsloten wordt hier ook het endpoint van elke dataset (zowel view als download) opgenomen. | http://inspirelab.geonovum.nl/test/rws/wms?request=GetCapabilities |
| **Protocol**  									| MD_Metadata.distributionInfo> MD_Distribution.transferOptions> MD_DigitalTransferOptions.onLine> CI_OnlineResource.protocol| Ja | Verplicht als er een URL is opgegeven. | xlink:href="http://www.opengis.net/def/serviceType/ogc/wms" OGC:WMS |
| **Applicatieprofiel**  							| MD_Metadata.distributionInfo> MD_Distribution.transferOptions> MD_DigitalTransferOptions.onLine> CI_OnlineResource.applicationProfile | Ja | Aanbevolen voor eenvoudigere dataservice-koppeling INSPIRE, hiermee wordt aangegeven dat aan betreffende technische specificatie wordt voldaan. Kies een waarde uit http://inspire.ec.europa.eu/metadata-codelist/SpatialDataServiceType. | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/SpatialDataServiceType/download Downloaddienst|
| **Naam**  										| MD_Metadata.distributionInfo> MD_Distribution.transferOptions> MD_DigitalTransferOptions.onLine> CI_OnlineResource.name| Ja | Het is verplicht als het protocol één van de volgende waardes heeft: OGC:WMS, OGC:WFS, OGC:WMTS, OGC:WCS en INSPIRE:Atom.| Gemeentegrenzen |
| **Omschrijving**  								| MD_Metadata.distributionInfo> MD_Distribution.transferOptions> MD_DigitalTransferOptions.onLine> CI_OnlineResource.description | | Aanbevolen dit zowel voor endPoints als ook voor accessPoints op te nemen, is nog geen duidelijkheid voor de eenvoudigere dataservice-koppeling INSPIRE| xlink:href="http://inspire.ec.europa.eu/metadata-codelist/OnLineDescriptionCode/accessPoint accessPoint|
| **Trefwoord** 									| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.keyword| Ja | INSPIRE vereist dat de naam van het thema als trefwoord wordt opgenomen uit de GEMET INSPIRE themes thesaurus | Hydrografie |
| **Naam van Thesaurus**  							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.title| Ja |Verplichte thesaurus voor INSPIRE | GEMET - INSPIRE themes, version 1.0|
| **Thesaurusdatum**  								| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.date| Ja | De datum van publicatie van de INSPIRE thema thesaurus | 2008-06-01 |
| **Thesaurus-datumtype** 							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.dateType| Ja | Het datumtype | publicatie |
| **Trefwoord** 									| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.keyword| Ja | INSPIRE vereist voor monitoring dat een trefwoord met de waarde *nationaal*, *regionaal* of *lokaal* voor ruimtelijke dekking wordt opgenomen uit de de codelijst http://inspire.ec.europa.eu/metadata-codelist/SpatialScope/ | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/SpatialScope/national Nationaal |
| **Naam van Thesaurus**  							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.title| Ja | Verplichte thesaurus voor ruimtelijke dekking van datasets INSPIRE. | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/SpatialScope Ruimtelijke dekking |
| **Thesaurusdatum**  								| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.date| Ja | De datum van publicatie van de codelijst.| 2019-05-22 |
| **Thesaurus-datumtype** 							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.dateType| Ja | Het datumtype | publicatie |
| **Trefwoord** 									| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.keyword| Ja | INSPIRE vereist voor prioritaire datasets dat een trefwoord wordt opgenomen uit de de codelijst http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset/AirQualityMonitoringStationsData-dir-2008-50 Monitoring stations (Richtlijn Luchtkwaliteit)|
| **Naam van Thesaurus**  							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.title| Ja | Verplichte thesaurus voor prioritaire datasets INSPIRE.| xlink:href="http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset INSPIRE prioritaire dataset|
| **Thesaurusdatum**  								| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.date| Ja | De datum van publicatie van de codelijst.| 2018-04-04 |
| **Thesaurus-datumtype** 							| MD_Metadata.identificationInfo> MD_DataIdentification.descriptiveKeywords> MD_Keywords.thesaurusName> CI_Citation.date> CI_Date.dateType| Ja | Het datumtype | publicatie |
| **Overige beperkingen**  							| MD_Metadata.identificationInfo[1]/\*/resourceConstraints/\*/otherConstraint | Ja | Voor INSPIRE moet een waarde uit codelijst ConditionsApplyingToAccessAndUse worden opgegeven | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/ConditionsApplyingToAccessAndUse/noConditionsApply Geen beperkingen|
| **Overige beperkingen**  							| MD_Metadata.identificationInfo[1]/\*/resourceConstraints/\*/otherConstraint | Ja | Voor INSPIRE moet ook een waarde uit codelijst LimitationsOnPublicAccess worden opgegeven | xlink:href="http://inspire.ec.europa.eu/metadata-codelist/LimitationsOnPublicAccess/noLimitations Geen beperkingen|
| **Ruimtelijk schema** 							| MD_Metadata.identificationInfo[1]/*/spatialRepresentationType | Ja | Voor INSPIRE moet ook een waarde uit codelijst SpatialRepresentationTypeCode worden opgegeven | vector |
| **Naam distributieformaat**  						| MD_Metadata.distributionInfo> MD_Distribution.distributionFormat> MD_Format.name| C | Het verplicht als de dataset een geharmoniseerde INSPIRE dataset is. | xlink:href="http://inspire.ec.europa.eu/schemas/hy/4.0/HydroBase.xsd Hydrography GML application schema|
| **Versie distributieformaat**  					| MD_Metadata.distributionInfo> MD_Distribution.distributionFormat> MD_Format.version| C | Het is verplicht als de dataset een geharmoniseerde INSPIRE dataset is. | version 3.0; GML, version 3.2. |
| **Specificatie distributieformaat**  				| MD_Metadata.distributionInfo> MD_Distribution.distributionFormat> MD_Format.specification| C | Het is verplicht als de dataset een geharmoniseerde INSPIRE dataset is. | xlink:href=http://inspire.ec.europa.eu/id/document/tg/hy Dataspecificatie hydrografie|
| **Specificatie titel** 							| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[1]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.title| Ja | Hiermee word aangegeven dat de data volgens de INSPIRE-verordening is. Voor as-is datasets op false zetten. Voor alle thema's is dit verplicht om op te nemen. | VERORDENING (EU) Nr. 1089/2010 VAN DE COMMISSIE van 23 november 2010 ter uitvoering van Richtlijn 2007/2/EG van het Europees Parlement en de Raad betreffende de interoperabiliteit van verzamelingen ruimtelijke gegevens en van diensten met betrekking tot ruimtelijke gegevens |
| **Specificatie datum**  							| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[1]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.date> CI_Date.date| Ja | Publicatiedatum van de Inspire-verordening | 2010-12-08 |
| **Specificatie datumtype**  						| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.date> CI_Date.dateType| Ja | | publicatie |
| **Verklaring**  									| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.explanation| Ja | | |
| **Indicatie van conformiteit met de specificatie**| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.pass| Ja | Zie annex A van de dataspecificaties voor de conformiteitsvereisten | vinkje true / false |
| **Specificatie titel** 							| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[2]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.title| Ja | Hiermee kan de conformiteit met de technische specificaties worden aangegeven | xlink:href="http://inspire.ec.europa.eu/id/document/tg/au Data specificatie administratieve eenheden|
| **Specificatie datum**  							| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[2]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.date> CI_Date.date| Ja | Publicatiedatum van de versie van de INSPIRE-dataspecificatie die gebruikt is.| 2010-05-03 |
| **Specificatie datumtype**  						| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.specification> CI_Citation.date> CI_Date.dateType| Ja | | publicatie |
| **Verklaring**  									| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.explanation| Ja | | |
| **Indicatie van conformiteit met de specificatie**| MD_Metadata.dataQualityInfo> DQ_DataQuality.report[*]> DQ_DomainConsistency.result> DQ_ConformanceResult.pass| Ja | Zie annex A van de dataspecificaties voor de conformiteitsvereisten | vinkje true / false |
| **Type waarde**  									| MD_Metadata.dataQualityInfo> DQ_DataQuality.report> DQ_TopologicalConsistency.result> DQ_QuantitativeResult.valueUnit| C | Verplicht voor INSPIRE-datasets als voor netwerken de aansluiting van hartlijnen niet is verzekerd.| cm |
| **Topologische samenhang**  						| MD_Metadata.dataQualityInfo> DQ_DataQuality.report> DQ_TopologicalConsistency.result> DQ_QuantitativeResult.value| C | Verplicht voor INSPIRE-datasets als voor netwerken de aansluiting van hartlijnen niet is verzekerd.| 3 |
| **Rol organisatie metadata** 						| MD_Metadata.contact> CI_ResponsibleParty.role| Ja | Het betreft de rol van de organisatie. Inspire verplicht hier om *contactpunt* in te vullen. | contactpunt |

### Aandachtspunten
De elementen van Specificatie en trefwoorden worden meerdere keren opgenomen. Voor alle thema's is het opgeven van de conformiteit met de verordening verplicht. Daarnaast zijn er INSPIRE-conformiteit-vereisten opgenomen in Annex A van de dataspecificaties voor de Annex II- en III-thema's. Daarbij is uitgegaan van het opgeven van de conformiteit van (delen van) de technische specificatie.

## Prioritaire datasets
Voor de prioritaire datasets zijn er aanvullende vereisten voor de metadata. Voor elke *directive* waar de data voor gebruikt wordt, wordt een trefwoord toegevoegd. Deze trefwoorden komen uit de bij het JRC beheerde INSPIRE-registry.

De trefwoorden kunnen volgens twee scenario's worden toegevoegd:

- **Scenario 1**: trefwoord en thesaurus worden toegevoegd zonder URI's. Hiervoor zijn geen handmatige aanpassingen in XML nodig.
- **Scenario 2**: trefwoord en thesaurus worden toegevoegd met URI's. Deze manier wordt aanbevolen en sluit al aan op methodes in het NL-metadataprofiel versie 2.0 en de recentste INSPIRE technical guidelines van metadata. Hiervoor is tijdelijk, tot overgang naar NL profiel versie 2.0 eenmalig een handmatige aanpassing in XML nodig.

### Scenario zonder URI's
De volgende acties zijn nodig wanneer trefwoord en thesaurus worden toegevoegd zonder URI's:
1. Ga naar de INSPIRE Registry (http://inspire.ec.europa.eu/registry).
2. Ga naar de prioritaire-dataset-metadata-codelijst (http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset).
3. Ga naar de betreffende prioritaire dataset.
4. Kopieer het NL-label.
5. Voeg deze als trefwoord toe aan de metadata samen met de verwijzing naar de thesaurus met *titel*, *datum* en *type datum*.
6. Als de dataset voor meerdere rapportage verplichtingen wordt gebruikt, voor elke verplichting de juiste trefwoorden zoeken en toevoegen.
7. Bewaar de aanpassingen en valideer je metadata. Er is (nog) geen test op deze extra trefwoorden.

**Voorbeeld voor dit scenario**
<pre class="xml">
&lt;!-- Trefwoord voor reporting verplichting voor INSPIRE --&gt;
&lt;gmd:descriptiveKeywords&gt;
&lt;gmd:MD_Keywords&gt;
    &lt;gmd:keyword&gt;
      &lt;gco:CharacterString&gt;Monitoring stations (Richtlijn Luchtkwaliteit)&lt;/gco:CharacterString&gt;
    &lt;/gmd:keyword&gt;
&lt;!-- Eventueel hier een tweede trefwoord voor tweede reporting verplichting voor INSPIRE --&gt;
    &lt;gmd:thesaurusName&gt;
      &lt;gmd:CI_Citation&gt;
        &lt;gmd:title&gt;
          &lt;gco:CharacterString&gt;INSPIRE prioritaire dataset&lt;/gco:CharacterString&gt;
        &lt;/gmd:title&gt;
        &lt;gmd:date&gt;
          &lt;gmd:CI_Date&gt;
            &lt;gmd:date&gt;
              &lt;gco:Date&gt;2018-04-04&lt;/gco:Date&gt;
            &lt;/gmd:date&gt;
            &lt;gmd:dateType&gt;
              &lt;gmd:CI_DateTypeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"/&gt;
            &lt;/gmd:dateType&gt;
          &lt;/gmd:CI_Date&gt;
        &lt;/gmd:date&gt;
      &lt;/gmd:CI_Citation&gt;
    &lt;/gmd:thesaurusName&gt; 
  &lt;/gmd:MD_Keywords&gt;
&lt;/gmd:descriptiveKeywords&gt;
</pre>

### Scenario met URI's
De volgende acties zijn nodig wanneer trefwoord en thesaurus worden toegevoegd mét URI's:
1. Ga naar de INSPIRE Registry (http://inspire.ec.europa.eu/registry).
2. Ga naar de prioritaire-dataset-metadata-codelijst (http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset).
3. Ga naar de betreffende prioritaire dataset.
4. Kopieer de URI en het NL-label.
5. Voeg deze als trefwoord toe aan de metadata samen met de verwijzing naar de thesaurus met *titel*, *datum* en *type datum*. Hiervoor kan onderstaande XML-voorbeeld in de XML worden gekopieerd.
6. Als de dataset voor meerdere rapportageverplichtingen wordt gebruikt, voor elke verplichting de juiste trefwoorden zoeken en toevoegen.
7. Neem bovenin de XML de namespace en schemalocatie van GMX op als volgt:
<pre class="xml">
&lt;gmd:MD_Metadata
  xmlns:gml="http://www.opengis.net/gml"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:gmd="http://www.isotc211.org/2005/gmd"
  xmlns:gmx="http://www.isotc211.org/2005/gmx"
  xmlns:gts="http://www.isotc211.org/2005/gts"
  xmlns:gco="http://www.isotc211.org/2005/gco"
  xmlns:xlink="http://www.w3.org/1999/xlink"
  xsi:schemaLocation="http://www.isotc211.org/2005/gmd http://schemas.opengis.net/iso/19139/20060504/gmd/gmd.xsd
  http://www.isotc211.org/2005/gmx http://schemas.opengis.net/iso/19139/20060504/gmx/gmx.xsd"&gt;
</pre>
8. Bewaar de aanpassingen en valideer je metadata. Er is (nog) geen test op deze extra trefwoorden.

**Voorbeeld voor dit scenario**

<pre class="xml">
&lt;!-- Trefwoord voor reporting verplichting voor INSPIRE --&gt;
&lt;gmd:descriptiveKeywords&gt;
  &lt;gmd:MD_Keywords&gt;
    &lt;gmd:keyword&gt;
      &lt;gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset/AirQualityMonitoringStationsData-dir-2008-50"&gt;Monitoring stations (Richtlijn Luchtkwaliteit)&lt;/gmx:Anchor&gt;
    &lt;/gmd:keyword&gt;
&lt;!-- Eventueel hier een tweede trefwoord voor tweede reporting verplichting voor INSPIRE --&gt;
    &lt;gmd:thesaurusName&gt;
      &lt;gmd:CI_Citation&gt;
        &lt;gmd:title&gt;
          &lt;gmx:Anchor xlink:href="http://inspire.ec.europa.eu/metadata-codelist/PriorityDataset"&gt;INSPIRE prioritaire dataset&lt;/gmx:Anchor&gt;
        &lt;/gmd:title&gt;
        &lt;gmd:date&gt;
          &lt;gmd:CI_Date&gt;
            &lt;gmd:date&gt;
              &lt;gco:Date&gt;2018-04-04&lt;/gco:Date&gt;
            &lt;/gmd:date&gt;
            &lt;gmd:dateType&gt;
              &lt;gmd:CI_DateTypeCode codeList="http://www.isotc211.org/2005/resources/Codelist/gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"/&gt;
            &lt;/gmd:dateType&gt;
          &lt;/gmd:CI_Date&gt;
        &lt;/gmd:date&gt;
      &lt;/gmd:CI_Citation&gt;
    &lt;/gmd:thesaurusName&gt; 
  &lt;/gmd:MD_Keywords&gt;
&lt;/gmd:descriptiveKeywords&gt;
</pre>

### Voorbeeldbestand prioritaire datasets
[Hier is een voorbeeldbestand waarin beide scenario's zijn uitgewerkt](https://wiki.geonovum.nl/images/Voorbeeld_XML_prioritaire_dataset.xml).

## Voorbeeldbestand XML voor INSPIRE dataset-metadata

Hier is een [voorbeeld-metadatabestand](https://wiki.geonovum.nl/images/Voorbeeld_Metadata_Dataset_2019.zip) te vinden voor een fictive dataset.

## Metadata-validatie
Validatie is een mechanisme om te controleren of een bepaalde metadatabeschrijving aan de specificaties voldoet. Het is een onmisbaar hulpmiddel om tot een correcte implementatie te komen. Er zijn verschillende validatietools beschikbaar om (verschillende onderdelen van) INSPIRE-metadata te valideren. Zie hiervoor [het hoofdstuk validatie](#validatie).

## FAQ metadata
**Vraag: Is mijn metadata conform INSPIRE als mijn metadata ISO 19115 volgt?**

INSPIRE volgt bestaande internationale standaarden, maar metadata die volledig conform ISO 19115 is voldoet niet aan de INSPIRE Implementing Rule Metadata. Op een aantal elementen is INSPIRE strikter dan de ISO: het zijn delen waarin de wetgeving bepaalde metadata-informatie verplicht stelt.

**Vraag: Welke validator moet gebruikt worden voor de INSPIRE-conformiteitstoetsen?**

Voor de INSPIRE-conformiteittoetsen voor metadata kan men gebruik maken van de Europese [INSPIRE-validators](https://inspire.ec.europa.eu/validator/).

**Vraag: Waarom kan ik mijn metadata niet in het EU INSPIRE portaal terugvinden?**

Alleen metadata met de aanduiding 'categorie INSPIRE' wordt doorgeleverd aan de EU voor INSPIRE. In het hoofstuk [Publiceren](#publiceren) is beschreven hoe dat uitgevoerd kan worden.

**Vraag: Trefwoord uit GEMET INSPIRE thema. Is een trefwoord verplicht in het metadatadocument?**

Voor datasets en dataset-series die onder INSPIRE vallen, dient men de thema’s waar de data onder valt op te nemen. Deze INSPIRE-thema’s zijn te vinden in de [thesaurus GEMET](http://www.eionet.europa.eu/gemet/inspire_themes). Voor INSPIRE moet tenminste één trefwoord uit deze thesaurus over worden genomen. Het is ook mogelijk daarnaast zelfgedefinieerde trefwoorden, of trefwoorden uit een andere thesaurus in te vullen.

Een voorbeeld:
<pre class="xml">
&lt;gmd:descriptiveKeywords&gt;
   &lt;gmd:MD_Keywords&gt;
      &lt;gmd:keyword&gt;
          &lt;gco:CharacterString&gt;infoMapAccessService&lt;/gco:CharacterString&gt;
     &lt;/gmd:keyword&gt;
   &lt;/gmd:MD_Keywords&gt;
&lt;/gmd:descriptiveKeywords&gt;

&lt;gmd:descriptiveKeywords&gt;
   &lt;gmd:MD_Keywords&gt;
       &lt;gmd:keyword&gt;
          &lt;gco:CharacterString&gt;Beschermde gebieden&lt;/gco:CharacterString&gt;
       &lt;/gmd:keyword&gt;
       &lt;gmd:thesaurusName&gt;
           &lt;gmd:CI_Citation&gt;
                &lt;gmd:title&gt;
                     &lt;gco:CharacterString&gt;GEMET - INSPIRE themes, version 1.0&lt;/gco:CharacterString&gt;
                &lt;/gmd:title&gt;
       .......
   &lt;/gmd:MD_Keywords&gt;
&lt;/gmd:descriptiveKeywords&gt;
</pre>

**Vraag: Is thesaurus titel, datum en datum type verplicht (thesaurusName element)?**

Nee, het thesaurusName element is een conditioneel element. Het is verplicht als er een trefwoord wordt opgenomen afkomstig uit een thesaurus. Het bevat dan de naam van de thesaurus waar het trefwoord uit afkomstig is.

Een voorbeeld:

<pre class="xml">
&lt;gmd:thesaurusName&gt;
   &lt;gmd:CI_Citation&gt;
      &lt;gmd:title&gt;
        &lt;gco:CharacterString&gt;GEMET - INSPIRE themes, version 1.0&lt;/gco:CharacterString&gt;
      &lt;/gmd:title&gt;
      &lt;gmd:date&gt;
         &lt;gmd:CI_Date&gt;
             &lt;gmd:date&gt;
                  &lt;gco:Date&gt;2008-06-01&lt;/gco:Date&gt;
             &lt;/gmd:date&gt;
             &lt;gmd:dateType&gt;
                 &lt;gmd:CI_DateTypeCode codeList="http://standards.iso.org/ittf/PubliclyAvailableStandards/ISO_19139_Schemas/resources/Codelist/ML_gmxCodelists.xml#CI_DateTypeCode" codeListValue="publication"&gt;publication&lt;/gmd:CI_DateTypeCode&gt;
             &lt;/gmd:dateType&gt;
         &lt;/gmd:CI_Date&gt;
      &lt;/gmd:date&gt;
   &lt;/gmd:CI_Citation&gt;
&lt;/gmd:thesaurusName&gt;
</pre>

**Vraag: Is het mogelijk ook zelf gedefinieerde trefwoorden in te vullen?**

Het is ook mogelijk zelfgedefinieerde trefwoorden, of trefwoorden uit een andere thesaurus in te vullen. Als de trefwoorden uit een thesaurus komen, dient thesaurus, datum en datum type gemeld te worden.

Een voorbeeld:

<pre class="xml">
&lt;gmd:descriptiveKeywords&gt;
    &lt;gmd:MD_Keywords&gt;
      &lt;gmd:keyword&gt;
         &lt;gco:CharacterString&gt;Ruimtegebruik&lt;/gco:CharacterString&gt;
      &lt;/gmd:keyword&gt;
      &lt;gmd:keyword&gt;
         &lt;gco:CharacterString&gt;Planologie&lt;/gco:CharacterString&gt;
      &lt;/gmd:keyword&gt;
   &lt;/gmd:MD_Keywords&gt;
</pre>

**Vraag: Is de metadata-taal een verplicht element?**

Ja, het metadata-taalelement is verplicht. In dit element wordt vastgelegd in welke taal de metadata is beschreven. Gebruik hiervoor alleen de drie-letter codes van 639-2/B (bibliographic codes), zoals gedefinieerd op http://www.loc.gov/standards/iso639-2/. Voor Nederlands is de code dut.

Een voorbeeld:

<pre class="xml">
&lt;gmd:language&gt;
   &lt;gmd:LanguageCode codeList="http://www.loc.gov/standards/iso639-2/" codeListValue="dut"&gt;Nederlands&lt;/gmd:LanguageCode&gt;
&lt;/gmd:language>
</pre>
