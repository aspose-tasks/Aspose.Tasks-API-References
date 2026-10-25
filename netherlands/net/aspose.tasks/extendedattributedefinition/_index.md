---
title: "Klasse ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ExtendedAttributeDefinition‑klasse. Vertegenwoordigt een definitie van een uitgebreid attribuut dat aan een project is gekoppeld"
type: docs
weight: 540
url: /nl/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Stelt een definitie van een uitgebreid attribuut voor dat aan een project is gekoppeld.

```csharp
public class ExtendedAttributeDefinition
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Haalt op of stelt de alias van een aangepast veld in. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of nieuwe waarden die aan een project worden toegevoegd automatisch aan de lijst worden toegevoegd. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of een automatische doorrol naar toewijzingen is ingeschakeld. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Haalt op of stelt het type berekening van de waarde van het aangepaste attribuut in. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Haalt het type van een aangepast veld op. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Haalt op of stelt de standaardwaarde in de lijst in. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Haalt op of stelt de Guid van de standaard opzoektabel‑vermelding in. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Haalt op of stelt in of het uitgebreide attribuut is gekoppeld aan een taak, een resource of een toewijzing. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Haalt op of stelt overeen met de project‑id van een aangepast veld. Gebruik de tekenreeksrepresentatie van een constante uit de [`ExtendedAttributeTask`](../extendedattributetask/)‑klasse om de [`FieldId`](./fieldid/)‑eigenschap op te geven. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Haalt de naam van een aangepast veld op. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Haalt de formule op of stelt deze in die Microsoft Project gebruikt om een aangepast taakveld te vullen. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Haalt de informatie over grafische indicatoren op of stelt deze in die aan het uitgebreide attribuut is gekoppeld. Van toepassing op MPP-indeling. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Haalt de GUID van een aangepast veld op of stelt deze in. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Haalt de GUID van de opzoektabel op die aan een aangepast veld is gekoppeld. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Haalt het maximum aantal waarden op of stelt dit in dat u in een keuzelijst kunt instellen. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Haalt het bovenliggende project op voor de `ExtendedAttributeDefinition`-instantie. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Haalt de fonetische uitspraak van de alias van een aangepast veld op of stelt deze in. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de waarden van het aangepaste veld beperkt zijn tot waarden in de [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Haalt de manier waarop roll-ups worden berekend op of stelt deze in. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Haalt de secundaire GUID van het uitgebreide attribuut op of stelt deze in. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Haalt de secundaire PID van een aangepast veld op of stelt deze in. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Haalt het type berekening van de waarde van het aangepaste attribuut voor samenvattingsrijen op of stelt dit in. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of een aangepast veld door de gebruiker is gedefinieerd. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Haalt de List&lt;Value&gt; ValueList op. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Haalt de manier waarop waardelijsten worden gesorteerd op of stelt deze in. Waarden zijn: 0=Aflopend, 1=Oplopend. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Factory-methode die een uitgebreide attribuutdefinitie met opzoeking maakt. Het heeft [`CalculationType`](./calculationtype/) gelijk aan Lookup en kan alleen in Resources worden gebruikt. U moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld-id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory-methode die een uitgebreide attribuutdefinitie met opzoeking maakt. Het heeft [`CalculationType`](./calculationtype/) gelijk aan Lookup en kan alleen in Resources worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Factory-methode die een uitgebreide attribuutdefinitie met opzoeking maakt. Het heeft [`CalculationType`](./calculationtype/) gelijk aan Lookup en kan alleen in Tasks worden gebruikt. U moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld-id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory-methode die een uitgebreide attribuutdefinitie met opzoeking maakt. Het heeft [`CalculationType`](./calculationtype/) gelijk aan Lookup en kan alleen in Tasks worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\". Het heeft [`CalculationType`](./calculationtype/) gelijk aan None en kan alleen in Resource worden gebruikt. U moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld-id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\". Het heeft [`CalculationType`](./calculationtype/) gelijk aan None en kan alleen in Resource worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\". Het heeft [`CalculationType`](./calculationtype/) gelijk aan None en kan alleen in Tasks worden gebruikt. U moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld-id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory-methode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als \"None\". Het heeft [`CalculationType`](./calculationtype/) gelijk aan None en kan alleen in Tasks worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Voegt een waarde toe aan de interne opzoektabel. Dit is een voorkeursmethode voor manipulaties met de [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven vlagwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven datumwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven numerieke waarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven duurwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Maakt een nieuw uitgebreid attribuut met de veld-ID die gelijk is aan de veld-ID-waarde van dit object en de opgegeven tekstwaarde. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Maakt een nieuw uitgebreid attribuut gekoppeld aan het opgegeven [`Value`](../value/)‑item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Retourneert een vlag die aangeeft of deze instantie gelijk is aan het opgegeven object. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Retourneert een hashcode voor de instantie van de `ExtendedAttributeDefinition`‑klasse. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Verwijdert een waarde uit de interne opzoeklijst. Dit is een voorkeursmethode voor manipulaties met de [`ValueList`](./valuelist/). |

## Voorbeelden

Toont hoe je algemene wiskundige functies gebruikt met uitgebreide attributen.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Formule instellen
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Print uitgebreide attribuutwaarde
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Formule instellen
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Print uitgebreide attribuutwaarde
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Formule instellen
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Print uitgebreide attribuutwaarde
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


