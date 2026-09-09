---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Bir OutlineCodeCollection nesnesi alır. Bir outline kodunun değeri"
type: docs
weight: 540
url: /tr/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

OutlineCodeCollection nesnesini alır. Bir taslak kodunun değerini.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Açıklamalar

İki veri parçası gereklidir - FieldID tarafından belirtilen outline kod tablosuna bir işaretçi ve değerin ValueID veya ValueGUID işaretçisiyle belirtilen değer listesi.

## Örnekler

Kaynak outline değerleriyle nasıl çalışılacağını gösterir.

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

### Ayrıca Bakınız

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


