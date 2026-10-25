---
title: "PropertyKeyedCollection1.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "PropertyKeyedCollection method. Crea una nuova proprietà personalizzata"
type: docs
weight: 50
url: /it/net/aspose.tasks.properties/propertykeyedcollection-1/add/
---
## PropertyKeyedCollection&lt;T&gt;.Add method

Crea una nuova proprietà personalizzata.

```csharp
public void Add(T item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | T | La proprietà da aggiungere. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../)
* namespace [Aspose.Tasks.Properties](../../propertykeyedcollection-1/)
* assembly [Aspose.Tasks](../../../)


