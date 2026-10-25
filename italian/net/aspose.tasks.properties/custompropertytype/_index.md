---
title: "Enum CustomPropertyType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.Properties.CustomPropertyType. Rappresenta un'enumerazione di tipi di proprietà personalizzate"
type: docs
weight: 1560
url: /it/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

Rappresenta un'enumerazione del tipo di proprietà personalizzata.

```csharp
public enum CustomPropertyType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | La proprietà non ha tipo. |
| String | `1` | La proprietà è un valore stringa. |
| DateTime | `2` | La proprietà è un valore data/ora. |
| Number | `3` | La proprietà è un numero intero. |
| Boolean | `4` | La proprietà è un valore booleano. |

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


