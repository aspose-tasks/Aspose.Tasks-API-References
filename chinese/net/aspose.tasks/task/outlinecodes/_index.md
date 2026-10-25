---
title: "Task.OutlineCodes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取或设置 OutlineCodeCollection 对象"
type: docs
weight: 880
url: /zh/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

获取或设置 [`OutlineCodeCollection`](../../outlinecodecollection/) 对象。

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## 备注

需要两个数据项——由 FieldID 指定的大纲代码表指针，以及由 ValueID 或 ValueGUID 指定的值指针（指向值列表）。

## 示例

展示如何读取任务的轮廓代码值。

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

### 另见

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


