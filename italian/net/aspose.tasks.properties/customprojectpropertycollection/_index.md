---
title: "Classe CustomProjectPropertyCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Properties.CustomProjectPropertyCollection. Rappresenta una raccolta di proprietà personalizzate del progetto"
type: docs
weight: 1550
url: /it/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

Rappresenta una raccolta di proprietà di progetto personalizzate.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | Inizializza una nuova istanza della classe `CustomProjectPropertyCollection`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | Crea una nuova proprietà personalizzata. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | Crea una nuova proprietà personalizzata. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | Crea una nuova proprietà personalizzata. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | Crea una nuova proprietà personalizzata. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | Cancella la PropertyCollection. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | Rimuove una proprietà con il nome specificato dalla raccolta. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


