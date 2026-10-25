---
title: "Classe OutlineCodeCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineCodeCollection. Rappresenta una raccolta di oggetti OutlineCode"
type: docs
weight: 1160
url: /it/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

Rappresenta una raccolta di oggetti [`OutlineCode`](../outlinecode/).

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

## Esempi

Mostra come lavorare con le raccolte di codici outline.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// aggiungi una definizione di codice outline personalizzata
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// crea codice outline
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// si può verificare che la raccolta non sia di sola lettura
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// inserisci il codice con 2 in una posizione errata
task.OutlineCodes.Insert(0, code2);

// correggilo
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// inserisci il codice con 2 in una posizione corretta
task.OutlineCodes.Insert(2, code2);

// verifica che il codice sia stato inserito
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// lavora con i codici outline
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// aggiungi una definizione di codice outline personalizzata
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// crea codice outline
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// lavora con i codici outline
// ...

// rimuovi il codice outline
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// cancella tutti i valori contemporaneamente
task.OutlineCodes.Clear();
```

### Vedi anche

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


