---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Taakeigenschap. Haalt een OutlineCodeCollection-object op of stelt deze in"
type: docs
weight: 880
url: /nl/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Haalt een [`OutlineCodeCollection`](../../outlinecodecollection/) object op of stelt deze in.

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Opmerkingen

Twee gegevensstukken zijn nodig - een verwijzing naar de outline‑codetabel die wordt gespecificeerd door de FieldID, en de waarde die wordt gespecificeerd door ofwel de ValueID of de ValueGUID‑verwijzing naar de waardelijst.

## Voorbeelden

Toon hoe de outline‑codewaarden van een taak gelezen kunnen worden.

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

### Zie ook

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


