---
title: "结构体 KeyTK"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Key2TK 结构体。表示指定类型类的属性键。当获取或设置容器的属性时使用此类的实例。"
type: docs
weight: 930
url: /zh/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

表示指定类型的类的属性键。获取或设置容器属性时使用该类的实例。

```csharp
public struct Key<T, K>
    where K : struct
```

| 参数 | 描述 |
| --- | --- |
| T | 属性值的类型。 |
| K | 属性键的类型。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | 获取属性的键。 |

## 示例

展示如何读取/写入 Prj.ActualsInSync 属性。

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


