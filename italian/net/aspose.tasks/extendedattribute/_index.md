---
title: "Classe ExtendedAttribute"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ExtendedAttribute. Rappresenta gli attributi estesi"
type: docs
weight: 520
url: /it/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Rappresenta attributi estesi.

```csharp
public class ExtendedAttribute
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Ottiene la definizione dell'attributo. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Ottiene o imposta un valore per gli attributi con tipi data (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Ottiene o imposta il valore per gli attributi con tipo 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Ottiene l'ID di un campo. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Ottiene o imposta un valore che indica se un flag è impostato per un attributo con tipo 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Ottiene se il calcolo del valore dell'attributo esteso ha generato un errore. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Ottiene o imposta un valore per gli attributi con tipi numerici (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Ottiene o imposta un valore per gli attributi con tipo 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Ottiene il GUID di un valore di ricerca. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Ottiene un valore che indica se il valore di questa istanza `ExtendedAttribute` è di sola lettura. Restituisce true se una formula o rollup è definita nella [`ExtendedAttributeDefinition`](../extendedattributedefinition/) per questo oggetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Restituisce la rappresentazione stringa breve di un attributo esteso. |

## Osservazioni

Attualmente supportati tutti i tipi di attributi estesi letti da MSP Xml 2003/2007 e mpp 2003. Per MSP mpp 2007 tutti i letture di attributi estesi sono supportate eccetto durate e flag.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


