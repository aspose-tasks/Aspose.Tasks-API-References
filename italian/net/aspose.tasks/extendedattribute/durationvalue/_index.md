---
title: "ExtendedAttribute.DurationValue"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ExtendedAttribute. Ottiene o imposta il valore per gli attributi di tipo Durata"
type: docs
weight: 30
url: /it/net/aspose.tasks/extendedattribute/durationvalue/
---
## ExtendedAttribute.DurationValue property

Ottiene o imposta il valore per gli attributi con tipo 'Duration'.

```csharp
public Duration DurationValue { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| InvalidOperationException | Generato se la proprietà [`AttributeDefinition`](../attributedefinition/) non è inizializzata o il tipo di campo personalizzato della proprietà [`AttributeDefinition`](../attributedefinition/) non è un'istanza di [`Duration`](../../duration/). |

## Esempi

Mostra come aggiungere attributi estesi che utilizzano le formule di data/ora di MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Imposta la formula ProjDateDiff e stampa il valore dell'attributo esteso
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// Imposta la formula ProjDateSub e stampa il valore dell'attributo esteso
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Possiamo impostare la formula ProjDurConv su un attributo con valore di durata così come su un attributo con valore di testo.
// Imposta la formula ProjDurConv sull'attributo esteso con valore di durata e stampa il suo valore.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Imposta la formula ProjDurConv sull'attributo esteso con valore di testo e stampa il suo valore.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Imposta la formula Second e stampa il valore dell'attributo esteso
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Imposta la formula Weekday e stampa il valore dell'attributo esteso
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Vedi anche

* struct [Duration](../../duration/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


