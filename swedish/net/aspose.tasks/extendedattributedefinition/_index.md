---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks för .NET API-referens
description: Representerar en utökad attributdefinition associerad med ett projekt.
type: docs
weight: 530
url: /sv/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Representerar en utökad attributdefinition associerad med ett projekt.

```csharp
public class ExtendedAttributeDefinition
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Hämtar eller ställer in aliaset för ett anpassat fält. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Hämtar eller ställer in ett värde som anger om nya värden som läggs till ett projekt automatiskt läggs till i listan. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Hämtar eller ställer in ett värde som anger om en automatisk nedrullning till uppdrag är aktiverad. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Hämtar eller ställer in typen av beräkning av det anpassade attributets värde. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Hämtar typen av ett anpassat fält. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Hämtar eller ställer in standardvärdet i listan. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Hämtar eller ställer in guiden för standarduppslagstabellposten. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Hämtar eller ställer in det utökade attributet som är associerat med en uppgift, en resurs eller en tilldelning. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Hämtar eller sätter motsvarar projekt-id:t för ett anpassat fält. Använd strängrepresentation av en konstant från[`ExtendedAttributeTask`](../extendedattributetask) klass att specificera[`FieldId`](./fieldid) egenskap. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Hämtar namnet på ett anpassat fält. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Hämtar eller ställer in formeln som Microsoft Project använder för att fylla i ett anpassat uppgiftsfält. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Hämtar eller ställer in guiden för ett anpassat fält. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Får en guide över uppslagstabellen som är kopplad till ett anpassat fält. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Hämtar eller ställer in det maximala antalet värden du kan ange i en plocklista. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Hämtar det överordnade projektet för[`ExtendedAttributeDefinition`](../extendedattributedefinition) instans. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Hämtar eller ställer in det fonetiska uttalet av aliaset för ett anpassat fält. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Hämtar eller ställer in ett värde som anger om de anpassade fältvärdena är begränsade till värden i[`ValueList`](./valuelist) . |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Hämtar eller ställer in hur sammanslagningar beräknas. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Hämtar eller ställer in den sekundära guiden för utökat attribut. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Hämtar eller ställer in sekundär PID för ett anpassat fält. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Hämtar eller ställer in typen av beräkning av det anpassade attributets värde för sammanfattningsrader. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Hämtar eller ställer in ett värde som anger om ett anpassat fält är användardefinierat. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Hämtar List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Hämtar eller ställer in hur värdelistor sorteras. Värden är: 0=Fallande, 1=Stigande. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](./calculationtype) är lika medLookup och kan endast användas i Resurser. Du måste ange*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](./calculationtype) är lika medLookup och kan endast användas i Resurser. Du måste ange*customFieldType* ,*fieldId* och*alias* när anropa denna metod. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](./calculationtype) är lika medLookup och kan endast användas i Tasks. Du måste specificera*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Fabriksmetod som skapar en utökad attributdefinition med lookup. Den har[`CalculationType`](./calculationtype) är lika medLookup och kan endast användas i Tasks. Du måste specificera*customFieldType* ,*fieldId* och*alias* när anropa denna metod. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](./calculationtype) är lika medNone och kan endast användas i Resource. Du måste ange*fieldId* och*alias* när anropa denna metod. Fälttypen härleds från fält-id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](./calculationtype) är lika medNone och kan endast användas i Resource. Du måste ange*customFieldType* ,*fieldId* och*alias* när anropa denna metod. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](./calculationtype) är lika medNone och kan endast användas i Tasks. Du måste specificera*fieldId* och*alias* när den här metoden anropas. Fälttypen härleds från fält-id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Fabriksmetod som skapar en enkel utökad attributdefinition, som Microsoft Project visar som "Ingen". Den har[`CalculationType`](./calculationtype) är lika medNone och kan endast användas i Tasks. Du måste specificera*customFieldType* ,*fieldId* och*alias* när du anropar den här metoden. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Lägger till ett värde till den interna uppslagslistan. Detta är ett föredraget sätt för manipulationer med[`ValueList`](./valuelist) . |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna flaggvärdet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna datumvärdet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna numeriska värdet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna varaktighetsvärdet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Skapar ett nytt utökat attribut med fält-ID som är lika med detta objekts fält-ID-värde och det angivna textvärdet. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Skapar nytt utökat attribut kopplat till specificerad[`Value`](../value) item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Returnerar en flagga som anger om denna instans är lika med det angivna objektet. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Returnerar en hash-kod för instansen av[`ExtendedAttributeDefinition`](../extendedattributedefinition) class. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Tar bort ett värde från den interna uppslagslistan. Detta är ett föredraget sätt för manipulationer med[`ValueList`](./valuelist) . |

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
