---
title: "CustomProjectPropertyCollection.CustomProjectPropertyCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore CustomProjectPropertyCollection. Inizializza una nuova istanza della classe CustomProjectPropertyCollection"
type: docs
weight: 10
url: /it/net/aspose.tasks.properties/customprojectpropertycollection/customprojectpropertycollection/
---
## CustomProjectPropertyCollection constructor

Inizializza una nuova istanza della classe [`CustomProjectPropertyCollection`](../).

```csharp
public CustomProjectPropertyCollection()
```

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


