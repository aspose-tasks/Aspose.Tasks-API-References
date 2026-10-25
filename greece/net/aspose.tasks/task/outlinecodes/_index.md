---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Task. Λαμβάνει ή ορίζει το αντικείμενο OutlineCodeCollection"
type: docs
weight: 880
url: /el/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Λαμβάνει ή ορίζει το αντικείμενο [`OutlineCodeCollection`](../../outlinecodecollection/).

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Παρατηρήσεις

Απαιτούνται δύο στοιχεία δεδομένων - ένας δείκτης στον πίνακα outline code που καθορίζεται από το FieldID, και η τιμή που καθορίζεται είτε από το ValueID είτε από το ValueGUID δείκτη στη λίστα τιμών.

## Παραδείγματα

Δείξτε πώς να διαβάσετε τις τιμές κώδικα περιγράμματος της εργασίας.

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

### Δείτε επίσης

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


