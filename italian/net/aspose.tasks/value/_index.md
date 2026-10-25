---
title: "Classe Value"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Value. Rappresenta un valore in un elenco di valori"
type: docs
weight: 2800
url: /it/net/aspose.tasks/value/
---
## Value class

Rappresenta un valore in un elenco di valori.

```csharp
public class Value
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Value](value/)() | Inizializza una nuova istanza della classe `Value`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Ottiene o imposta il valore effettivo se può essere rappresentato come DateTime. Il valore predefinito è MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Ottiene o imposta la descrizione di un valore. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Ottiene o imposta il valore effettivo utilizzato per rappresentare la Durata. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Ottiene o imposta l'identificatore univoco di un valore all'interno di un progetto. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Ottiene o imposta il valore effettivo utilizzato per rappresentare un valore numerico o di costo. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Ottiene o imposta le informazioni fonetiche sul nome del campo personalizzato. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Ottiene o imposta il valore effettivo utilizzato per rappresentare una stringa di Text. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Ottiene o imposta il valore effettivo nella rappresentazione interna. Si consiglia di utilizzare le proprietà tipizzate fortemente elencate di seguito. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto. |

## Esempi

Mostra come leggere il lavoro con i valori di ricerca.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Crea una definizione di attributo esteso di tipo Testo
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Aggiungi valori di ricerca per la definizione di attributo esteso
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crea una definizione di attributo esteso di tipo Durata
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Aggiungi valori di ricerca per la definizione di attributo esteso
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crea una definizione di attributo esteso di tipo Data
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crea una definizione di attributo esteso di tipo Numero
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


