---
title: "ExtendedAttributeDefinition.CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ExtendedAttributeDefinition-methode. Fabriekmethode die een uitgebreide attribuutdefinitie met lookup maakt. Het heeft CalculationType gelijk aan Lookup en kan alleen in Taken worden gebruikt. U moet fieldId en alias opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld‑id."
type: docs
weight: 20
url: /nl/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Fabriekmethode die een uitgebreide attribuutdefinitie met lookup maakt. Het heeft [`CalculationType`](../calculationtype/) gelijk aan Lookup en kan alleen in Taken worden gebruikt. U moet *fieldId* en *alias* opgeven bij het aanroepen van deze methode. Het veldtype wordt afgeleid van het veld‑id.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Het opgegeven [`ExtendedAttributeTask`](../../extendedattributetask/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie voor een taak met lookup te maken en deze vervolgens te vullen met tekstwaarden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Toont hoe bijgewerkte uitgebreide attribuutdefinities te schrijven.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Voeg een nieuw uitgebreid attribuut text3 toe met een lookup en één lookup‑waarde
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// Voeg een nieuw uitgebreid attribuut cost1 toe met een lookup en twee kostenwaarden
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// Voeg een nieuwe taak toe en wijs de lookup‑waarde van het attribuut toe.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// Definieer een duur‑attribuut zonder lookup.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Voeg een nieuwe taak toe en wijs een duurwaarde toe aan het eerder gedefinieerde duur‑attribuut.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### Zie ook

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Fabriekmethode die een uitgebreide attribuutdefinitie met lookup maakt. Het heeft [`CalculationType`](../calculationtype/) gelijk aan Lookup en kan alleen in Taken worden gebruikt. U moet *customFieldType*, *fieldId* en *alias* opgeven bij het aanroepen van deze methode.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| customFieldType | CustomFieldType | Het opgegeven [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeTask | Het opgegeven [`ExtendedAttributeTask`](../../extendedattributetask/) veld-ID. |
| alias | String | De opgegeven String-alias. |

### Retourwaarde

Aangemaakt exemplaar van de [`ExtendedAttributeDefinition`](../) klasse met opgegeven *customFieldType*, *fieldId* en *alias*.

## Voorbeelden

Gebruik dit voorbeeld om een aangepaste velddefinitie voor een taak met lookup te maken en deze vervolgens te vullen met tekstwaarden:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Toont hoe u uitgebreide attributen met zoekopdrachten kunt toevoegen voor toewijzingen.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Wijs resource "1 TRG: Trade Group" toe aan "TASK 1" door een ResourceAssignment-object te maken.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Maak een aangepaste attribuutdefinitie met zoekopdracht.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Deze waarde is te zien in de weergave "Resource usage" van MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Maak een aangepaste attribuutdefinitie met zoekopdracht.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Deze waarde is te zien in de weergave "Task usage" van MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// verkeerde waarden kunnen later worden verwijderd
taskCostAttr.RemoveLookupValue(taskWrongValue);

// werken met project...
```

### Zie ook

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


