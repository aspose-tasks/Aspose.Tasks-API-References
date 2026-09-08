---
title: "Task.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-eigenschap. Haalt een ExtendedAttributeCollection-object op dat de waarden van een uitgebreid attribuut bevat"
type: docs
weight: 400
url: /nl/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Haalt een ExtendedAttributeCollection-object op dat de waarden van een uitgebreid attribuut bevat.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Opmerkingen

Twee gegevensstukken zijn nodig - een verwijzing naar de extended attribute-tabel die wordt gespecificeerd ofwel door de unieke ID of het Field ID, en de waarde die wordt gespecificeerd ofwel met de waarde, of een verwijzing naar de waardelijst.

## Voorbeelden

Toont hoe taakuitgebreide attributen te lezen.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Maak definitie van uitgebreid attribuut
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Haal taak met index nul op
var tsk = project.RootTask.Children.GetById(1);

// Voeg uitgebreid attribuut toe
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Ook kan de volgende korte syntaxis worden gebruikt: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Maak een Extended Attribute Definition van het type Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Voeg het toe aan de Extended Attributes-collectie van het project
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Maak een Extended Attribute van de Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Ken een waarde toe aan de gegenereerde Extended Attribute. Het type van het attribuut is "Text", de eigenschap "TextValue" moet worden gebruikt.
taskExtendedAttributeText1.TextValue = "London";

// Voeg de Extended Attribute toe aan de taak
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Maak een Extended Attribute Definition van het type Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Voeg het toe aan de Extended Attributes-collectie van het project
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Maak een Extended Attribute van de Text2 Lookup Definition voor Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Voeg de Extended Attribute toe aan de taak
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Maak een Extended Attribute Definition van het type Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Voeg de definitie toe aan de Extended Attributes-collectie van het project
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Maak een Extended Attribute van de Duration2 Lookup Definition voor Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Voeg de Extended Attribute toe aan de taak
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Maak een Extended Attribute Definition van het type Finish2 Type
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Voeg lookup-waarden toe voor de extended attribute definition
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Voeg de definitie toe aan de Extended Attributes-collectie van het project
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Maak een Extended Attribute van de Finish2 Lookup Definition voor Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Voeg de Extended Attribute toe aan de taak
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Lees uitgebreide attributen voor taken
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


