---
title: "Classe OutlineValueCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OutlineValueCollection. Rappresenta una collezione di oggetti OutlineValue"
type: docs
weight: 1220
url: /it/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

Rappresenta una collezione di oggetti [`OutlineValue`](../outlinevalue/).

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | Ottiene un valore che indica se questa collezione è di sola lettura. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

## Esempi

Mostra come lavorare con le collezioni di valori outline.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// cancella le collezioni di valori
foreach (var outlineCode in project.OutlineCodes)
{
    // cancella le maschere outline
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// aggiorna il valore tramite accesso per indice
codeDefinition.Values[0].Value = "654321";

// itera sui valori outline
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// lavora con i valori outline
// ...

// rimuovi un valore quando necessario
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// inserisci un valore nella posizione iniziale
codeDefinition.Values.Insert(0, value);

// verifica la posizione del valore inserito
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// lavora con i valori outline
// ...

// rimuovi l'ultimo valore dalla collezione
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// si può creare un'altra definizione di codice outline
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// e poi copiare i valori outline
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Vedi anche

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


