---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeDefinition. Rimuove un valore dall'elenco interno di ricerca. Questo è il modo preferibile per le manipolazioni con la ValueList"
type: docs
weight: 340
url: /it/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

Rimuove un valore dall'elenco interno di ricerca. Questo è il modo preferibile per le manipolazioni con la [`ValueList`](../valuelist/).

```csharp
public void RemoveLookupValue(Value value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | Valore | Valore da rimuovere dalla ricerca. |

## Osservazioni

Questo metodo funziona solo per le istanze di [`ExtendedAttributeDefinition`](../) che hanno [`CalculationType`](../calculationtype/) uguale a Lookup.

## Esempi

Mostra come aggiungere attributi estesi con ricerche per le assegnazioni.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Assegna la risorsa "1 TRG: Trade Group" al "TASK 1" creando un oggetto ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Crea una definizione di attributo personalizzato con ricerca.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Questo valore può essere visualizzato nella vista "Resource usage" di MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Crea una definizione di attributo personalizzato con ricerca.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Questo valore può essere visualizzato nella vista "Task usage" di MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// Valori errati possono essere rimossi in seguito.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// lavorare con il progetto...
```

### Vedi anche

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


