---
title: "OutlineCodeDefinitionCollection.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "OutlineCodeDefinitionCollection method. Copia gli elementi di questa collezione nell'array specificato a partire dall'indice specificato dell'array"
type: docs
weight: 70
url: /it/net/aspose.tasks/outlinecodedefinitioncollection/copyto/
---
## OutlineCodeDefinitionCollection.CopyTo method

Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato.

```csharp
public void CopyTo(OutlineCodeDefinition[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | OutlineCodeDefinition[] | l'array monodimensionale specificato a cui copiare gli elementi |
| arrayIndex | Int32 | l'indice basato su zero dell'array specificato al quale inizia la copia. |

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

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


