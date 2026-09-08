---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition methode. Fabriekmethode die een eenvoudige uitgebreide attribuutdefinitie maakt die Microsoft Project weergeeft als None. Het heeft CalculationType gelijk aan None en kan alleen in Tasks worden gebruikt. U moet customFieldType, fieldId en alias opgeven bij het aanroepen van deze methode"
type: docs
weight: 40
url: /nl/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Fabriekmethode die een eenvoudige uitgebreide attribuutdefinitie maakt, die Microsoft Project weergeeft als "None". Het heeft [`CalculationType`](../calculationtype/) gelijk aan None en kan alleen in Tasks worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| customFieldType | CustomFieldType | Het opgegeven [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeTask | Het opgegeven [`ExtendedAttributeTask`](../../extendedattributetask/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *customFieldType*, *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Toont hoe de uitgebreide attributen van een taak te maken.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Maak een Extended Attribute Definition van het type Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Voeg het toe aan de Extended Attributes-collectie van het project
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Voeg een taak toe aan het project
var task = project.RootTask.Children.Add("Task 1");

// Maak een Extended Attribute van de Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Ken een waarde toe aan de gegenereerde Extended Attribute. Het type van het attribuut is "Text", de eigenschap "TextValue" moet worden gebruikt.
taskExtendedAttributeText1.TextValue = "London";

// Voeg de Extended Attribute toe aan de taak
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Maak een Extended Attribute Definition van het type Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Voeg het toe aan de Extended Attributes-collectie van het project
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Voeg een taak toe aan het project
var task2 = project4.RootTask.Children.Add("Task 2");

// Maak een Extended Attribute van de Text2 Lookup Definition voor Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Voeg de Extended Attribute toe aan de taak
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Maak een Extended Attribute Definition van het type Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Voeg de definitie toe aan de Extended Attributes-collectie van het project
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Voeg een taak toe aan het project
var task3 = project2.RootTask.Children.Add("Task 3");

// Maak een Extended Attribute van de Duration2 Lookup Definition voor Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Voeg de Extended Attribute toe aan de taak
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Maak een Extended Attribute Definition van het type Finish2 Type
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Voeg de definitie toe aan de Extended Attributes-collectie van het project
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Voeg een taak toe aan het project
var task4 = project3.RootTask.Children.Add("Task 4");

// Maak een Extended Attribute van de Finish2 Lookup Definition voor Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Voeg de Extended Attribute toe aan de taak
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Factory-methode die een eenvoudige extended attribute definition maakt, die Microsoft Project weergeeft als "None". Het heeft [`CalculationType`](../calculationtype/) gelijk aan None en kan alleen in taken worden gebruikt. Je moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld-id.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Het opgegeven [`ExtendedAttributeTask`](../../extendedattributetask/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste tekstvelddefinitie te maken:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Toont hoe je een definitie van een uitgebreid attribuut maakt en een tekenreekswaarde voor het attribuut instelt tijdens de constructie.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// maak een uitgebreid attribuut met een waarde gelijk aan 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// voeg een uitgebreid attribuut toe geïnitialiseerd met de waarde 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### Zie ook

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


