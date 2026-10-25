---
title: "ExtendedAttribute.ValueReadOnly"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttribute. Ottiene un valore che indica se il valore di questa istanza di ExtendedAttribute è di sola lettura. Restituisce true se una formula o un rollup è definito in ExtendedAttributeDefinition per questo oggetto."
type: docs
weight: 100
url: /it/net/aspose.tasks/extendedattribute/valuereadonly/
---
## ExtendedAttribute.ValueReadOnly property

Ottiene un valore che indica se il valore di questa istanza di [`ExtendedAttribute`](../) è di sola lettura. Restituisce true se una formula o un rollup è definito in [`ExtendedAttributeDefinition`](../../extendedattributedefinition/) per questo oggetto.

```csharp
public bool ValueReadOnly { get; }
```

## Esempi

Mostra come aggiungere un campo personalizzato il cui valore è calcolato usando la formula specificata dall'utente.

```csharp
var project = new Project();

// crea una nuova definizione di attributo esteso per attività
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Aggiungi una formula all'attributo.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Crea attributo esteso
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Impostiamo la Formula per l'attributo esteso, così è di sola lettura (il valore è calcolato usando la formula).
// L'output è "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Puoi provare a impostare il valore di un campo di sola lettura, ma non avrà effetto.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Vedi anche

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


