---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource‑eigenschap. Haalt een OutlineCodeCollection-object op. De waarde van een outlinecode"
type: docs
weight: 540
url: /nl/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Haalt een OutlineCodeCollection-object op. De waarde van een outlinecode.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Opmerkingen

Twee gegevensstukken zijn nodig - een verwijzing naar de outline‑codetabel die wordt gespecificeerd door de FieldID, en de waarde die wordt gespecificeerd door ofwel de ValueID of de ValueGUID‑verwijzing naar de waardelijst.

## Voorbeelden

Toont hoe te werken met resource‑outline‑waarden.

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

### Zie ook

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


