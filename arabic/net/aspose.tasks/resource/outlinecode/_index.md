---
title: "Resource.OutlineCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. يحصل على كائن OutlineCodeCollection. قيمة رمز المخطط"
type: docs
weight: 540
url: /ar/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

يحصل على كائن OutlineCodeCollection. قيمة رمز المخطط.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## ملاحظات

هناك قطعتان من البيانات ضروريان - مؤشر إلى جدول رمز المخطط المحدد بواسطة FieldID، والقيمة المحددة إما بواسطة ValueID أو مؤشر ValueGUID إلى قائمة القيم.

## الأمثلة

يظهر كيفية العمل مع قيم مخطط المورد.

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

### انظر أيضًا

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


