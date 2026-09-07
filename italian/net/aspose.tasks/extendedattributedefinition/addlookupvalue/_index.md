---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeDefinition. Aggiunge un valore all'elenco interno di lookup. Questo è il modo consigliato per le manipolazioni con ValueList"
type: docs
weight: 300
url: /it/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Aggiunge un valore all'elenco interno di lookup. Questo è il modo consigliato per le manipolazioni con [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | Valore | Valore da aggiungere al lookup. |

## Osservazioni

Questo metodo funziona solo per le istanze di [`ExtendedAttributeDefinition`](../) che hanno [`CalculationType`](../calculationtype/) uguale a Lookup.

## Esempi

Utilizza questo codice per aggiungere un nuovo Valore all'elenco di lookup:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

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


