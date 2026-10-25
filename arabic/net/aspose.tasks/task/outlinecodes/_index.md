---
title: "Task.OutlineCodes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Task property. يحصل أو يعيّن كائن OutlineCodeCollection"
type: docs
weight: 880
url: /ar/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

يحصل أو يعيّن [`OutlineCodeCollection`](../../outlinecodecollection/) كائن.

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## ملاحظات

هناك قطعتان من البيانات ضروريان - مؤشر إلى جدول رمز المخطط المحدد بواسطة FieldID، والقيمة المحددة إما بواسطة ValueID أو مؤشر ValueGUID إلى قائمة القيم.

## الأمثلة

أظهر كيفية قراءة قيم رمز المخطط للـ task.

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

### انظر أيضًا

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


