---
title: "Project.Get"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。返回此容器中属性映射的值"
type: docs
weight: 1080
url: /zh/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

返回属性在此容器中映射的值。

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| 参数 | 描述 |
| --- | --- |
| T | 映射值的类型。 |
| key | 指定的属性键。[`Prj`](../../prj/) 用于获取属性键。 |

### 返回值

属性在此容器中映射的值。

## 示例

展示如何检查项目版本。

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// 显示项目版本
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


