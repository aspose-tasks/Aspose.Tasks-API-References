---
title: "Classe OutlineCodeDefinitionCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineCodeDefinitionCollection. Rappresenta una collezione di oggetti OutlineCodeDefinition."
type: docs
weight: 1180
url: /it/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Rappresenta una collezione di oggetti [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Converte questo oggetto OutlineCodeDefinitionCollection in un elenco di oggetti [`OutlineCodeDefinition`](../outlinecodedefinition/). |

## Esempi

Mostra come lavorare con le collezioni di definizioni di codici outline.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// aggiungi una definizione di codice outline personalizzata
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // inserisci la definizione di codice outline nella posizione
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// trova l'indice della definizione di codice outline
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// modifica la definizione del codice di contorno
project.OutlineCodes[index].Alias = "New Alias";

// ...
// lavora con le definizioni del codice di contorno
// ...

// rimuovi la definizione del codice di contorno
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// rimuovi una definizione del codice di contorno per indice
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// rimuovi le definizioni del codice di contorno
otherProject.OutlineCodes.Clear();

// copia le definizioni del codice di contorno
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// lavora con le definizioni del codice di contorno
// ...

// rimuovi le definizioni del codice di contorno una alla volta
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Vedi anche

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


