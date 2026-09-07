---
title: "Struttura GenericPropertyTKey"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Struttura Aspose.Tasks.Properties.GenericProperty1TKey. Rappresenta una proprietà contenitore"
type: docs
weight: 1570
url: /it/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Rappresenta una proprietà del contenitore.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Parametro | Descrizione |
| --- | --- |
| TKey | Il tipo del valore della proprietà. |

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Inizializza una nuova istanza della struttura `GenericProperty`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Ottiene il nome della proprietà. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Ottiene un valore della proprietà. |

## Esempi

Mostra come lavorare con le collezioni di proprietà di progetto personalizzate.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// aggiungiamo nuove proprietà personalizzate
// la collezione supporta i tipi Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// le proprietà personalizzate sono disponibili tramite la collezione tipizzata
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// ottieni il valore di una proprietà personalizzata
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// itera sui nomi delle proprietà personalizzate
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// è possibile eliminare un valore tramite chiave stringa
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// oppure si può cancellare completamente la collezione
project.CustomProps.Clear();
```

### Vedi anche

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


