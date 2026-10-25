---
title: "ExtendedAttribute.DateValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttribute. Ottiene o imposta un valore per gli attributi con tipi data Date Start Finish."
type: docs
weight: 20
url: /it/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

Ottiene o imposta un valore per gli attributi con tipi data (Date, Start, Finish).

```csharp
public DateTime DateValue { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generato se la proprietà [`AttributeDefinition`](../attributedefinition/) non è inizializzata o l'attributo corrente non è un attributo di tipo data. |

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


