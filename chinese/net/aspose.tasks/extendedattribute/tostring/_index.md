---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ExtendedAttribute 方法。返回扩展属性的简短字符串表示"
type: docs
weight: 110
url: /zh/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

返回扩展属性的简短字符串表示。

```csharp
public override string ToString()
```

### 返回值

扩展属性的字符串表示。

## 示例

展示如何读取扩展属性。

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 读取任务的扩展属性
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // 读取扩展属性的常用信息
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### 另见

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


