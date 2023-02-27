---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks voor .NET API-referentie
description: Vertegenwoordigt een uitgebreide kenmerkdefinitie die aan een project is gekoppeld.
type: docs
weight: 540
url: /nl/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Vertegenwoordigt een uitgebreide kenmerkdefinitie die aan een project is gekoppeld.

```csharp
public class ExtendedAttributeDefinition
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Haalt de alias van een aangepast veld op of stelt deze in. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of nieuwe waarden die aan een project worden toegevoegd, automatisch aan de lijst worden toegevoegd. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of een automatische roll-down naar toewijzingen is ingeschakeld. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Hiermee wordt het type berekening van de waarde van het aangepaste kenmerk opgehaald of ingesteld. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Krijgt het type van een aangepast veld. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Haalt of stelt de standaardwaarde in de lijst in. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Haalt de GUID van het standaard opzoektabelitem op of stelt deze in. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Haalt of stelt het uitgebreide attribuut is geassocieerd in met een taak, een resource of een opdracht. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Gets of sets komt overeen met de project-id van een aangepast veld. Gebruik tekenreeksrepresentatie van een constante uit[`ExtendedAttributeTask`](../extendedattributetask/) klasse te specificeren[`FieldId`](./fieldid/) eigenschap. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Krijgt de naam van een aangepast veld. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Hiermee wordt de formule opgehaald of ingesteld die Microsoft Project gebruikt om een aangepast taakveld in te vullen. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Haalt de GUID van een aangepast veld op of stelt deze in. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Haalt een GUID op van de opzoektabel die is gekoppeld aan een aangepast veld. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Haalt of stelt het maximale aantal waarden in dat u in een keuzelijst kunt instellen. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Haalt het bovenliggende project op voor het`ExtendedAttributeDefinition` instantie. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Hiermee wordt de fonetische uitspraak van de alias van een aangepast veld opgehaald of ingesteld. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de aangepaste veldwaarden beperkt zijn tot waarden in de[`ValueList`](./valuelist/) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Hiermee wordt de manier waarop rollups worden berekend opgehaald of ingesteld. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Haalt de secundaire GUID van uitgebreid attribuut op of stelt deze in. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Haalt de secundaire PID van een aangepast veld op of stelt deze in. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Hiermee wordt het type berekening van de waarde van het aangepaste kenmerk voor samenvattingsrijen opgehaald of ingesteld. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Haalt of stelt een waarde in die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Haalt de lijst op &lt;Waarde&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Hiermee wordt de manier waarop waardelijsten worden gesorteerd opgehaald of ingesteld. Waarden zijn: 0=Aflopend, 1=Oplopend. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](./calculationtype/) is gelijk aanLookup en kan alleen in Resources worden gebruikt. U bent verplicht om te specificeren*fieldId* En*alias* wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veld-id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](./calculationtype/) is gelijk aanLookup en kan alleen in Resources worden gebruikt. U bent verplicht om te specificeren*customFieldType* ,*fieldId* En*alias* wanneer deze methode wordt aangeroepen. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](./calculationtype/) is gelijk aanLookup en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*fieldId* En*alias* wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veld-id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Fabrieksmethode die een uitgebreide attribuutdefinitie creëert met lookup. Het heeft[`CalculationType`](./calculationtype/) is gelijk aanLookup en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*customFieldType* ,*fieldId* En*alias* wanneer deze methode wordt aangeroepen. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Fabrieksmethode die een eenvoudige uitgebreide attribuutdefinitie creëert, die Microsoft Project weergeeft als "Geen". Het heeft[`CalculationType`](./calculationtype/) is gelijk aanNone en kan alleen in Resource worden gebruikt. U bent verplicht om op te geven*fieldId* En*alias* wanneer deze methode wordt aangeroepen. Het veldtype wordt afgeleid uit veld-id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Fabrieksmethode die een eenvoudige uitgebreide attribuutdefinitie creëert, die Microsoft Project weergeeft als "Geen". Het heeft[`CalculationType`](./calculationtype/) is gelijk aanNone en kan alleen in Resource worden gebruikt. U bent verplicht om op te geven*customFieldType* ,*fieldId* En*alias* wanneer deze methode wordt aangeroepen. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Fabrieksmethode die een eenvoudige uitgebreide attribuutdefinitie creëert, die Microsoft Project weergeeft als "Geen". Het heeft[`CalculationType`](./calculationtype/) is gelijk aanNone en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*fieldId* En*alias* bij het aanroepen van deze methode. Het veldtype wordt afgeleid uit veld-ID. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Fabrieksmethode die een eenvoudige uitgebreide attribuutdefinitie creëert, die Microsoft Project weergeeft als "Geen". Het heeft[`CalculationType`](./calculationtype/) is gelijk aanNone en kan alleen in Tasks worden gebruikt. U bent verplicht om op te geven*customFieldType* ,*fieldId* En*alias* bij het aanroepen van deze methode. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Voegt een waarde toe aan de interne opzoeklijst. Dit is een voorkeursmanier voor manipulaties met de[`ValueList`](./valuelist/) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven vlagwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven duurwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Maakt een nieuw uitgebreid attribuut aan met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Creëert een nieuw uitgebreid attribuut gekoppeld aan opgegeven[`Value`](../value/) item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Retourneert een hash-code voor de instantie van het`ExtendedAttributeDefinition` klasse. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Verwijdert een waarde uit de interne opzoeklijst. Dit is een voorkeursmanier voor manipulaties met de[`ValueList`](./valuelist/) . |

### Zie ook

* naamruimte [Aspose.Tasks](../../aspose.tasks/)
* montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
