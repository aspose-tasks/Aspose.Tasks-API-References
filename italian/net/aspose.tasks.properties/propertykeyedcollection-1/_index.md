---
title: "Classe PropertyKeyedCollectionT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Properties.PropertyKeyedCollection1T. Una classe base di una raccolta di proprietà"
type: docs
weight: 1600
url: /it/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Una classe base di una raccolta di proprietà.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di proprietà. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Ottiene il numero di proprietà nella raccolta. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Ottiene la Proprietà associata alla chiave specificata. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Ottiene la raccolta di tutti i nomi delle proprietà. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Crea una nuova proprietà personalizzata. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Determina se la [`PropertyCollection`](../propertycollection-1/) contiene una proprietà con il nome specificato. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


