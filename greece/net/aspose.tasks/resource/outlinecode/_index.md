---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει ένα αντικείμενο OutlineCodeCollection. Η τιμή ενός outline code"
type: docs
weight: 540
url: /el/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Λαμβάνει ένα αντικείμενο OutlineCodeCollection. Η τιμή ενός κώδικα περιγράμματος.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Παρατηρήσεις

Απαιτούνται δύο στοιχεία δεδομένων - ένας δείκτης στον πίνακα outline code που καθορίζεται από το FieldID, και η τιμή που καθορίζεται είτε από το ValueID είτε από το ValueGUID δείκτη στη λίστα τιμών.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τις τιμές outline του πόρου.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### Δείτε επίσης

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


