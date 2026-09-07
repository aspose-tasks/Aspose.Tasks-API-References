---
title: "Task.OutlineCodes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene o imposta l'oggetto OutlineCodeCollection"
type: docs
weight: 880
url: /it/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Ottiene o imposta l'oggetto [`OutlineCodeCollection`](../../outlinecodecollection/).

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Osservazioni

Sono necessari due dati - un puntatore alla tabella dei codici di struttura specificata dal FieldID, e il valore specificato o dal puntatore ValueID o ValueGUID all'elenco dei valori.

## Esempi

Mostra come leggere i valori dei codici outline del task.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### Vedi anche

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


