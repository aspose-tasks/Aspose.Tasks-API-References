---
title: "Resource.OutlineCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取一个 OutlineCodeCollection 对象。大纲代码的值"
type: docs
weight: 540
url: /zh/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

获取 OutlineCodeCollection 对象。大纲代码的值。

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## 备注

需要两个数据项——由 FieldID 指定的大纲代码表指针，以及由 ValueID 或 ValueGUID 指定的值指针（指向值列表）。

## 示例

展示如何使用资源大纲值。

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

### 另见

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


