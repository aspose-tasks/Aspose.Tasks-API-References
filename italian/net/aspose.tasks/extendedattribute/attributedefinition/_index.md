---
title: "ExtendedAttribute.AttributeDefinition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttribute. Ottiene la definizione dell'attributo"
type: docs
weight: 10
url: /it/net/aspose.tasks/extendedattribute/attributedefinition/
---
## ExtendedAttribute.AttributeDefinition property

Ottiene la definizione dell'attributo.

```csharp
public ExtendedAttributeDefinition AttributeDefinition { get; }
```

## Esempi

Mostra come modificare la definizione dell'attributo esteso.

```csharp
var project = new Project();

// crea una nuova definizione di attributo esteso per attività
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// Aggiungi una formula all'attributo.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// Crea attributo esteso
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// crea una nuova definizione di attributo esteso di tipo data
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// Aggiungi una formula all'attributo.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### Vedi anche

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


