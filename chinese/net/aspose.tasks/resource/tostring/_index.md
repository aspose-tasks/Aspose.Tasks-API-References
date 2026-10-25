---
title: "Resource.ToString"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 方法。返回 Resource 类实例的简短字符串表示。表示的具体细节未指定，可能会更改。"
type: docs
weight: 870
url: /zh/net/aspose.tasks/resource/tostring/
---
## Resource.ToString method

返回 [`Resource`](../) 类实例的简短字符串表示。表示的具体细节未指定，可能会更改。

```csharp
public override string ToString()
```

### 返回值

表示资源对象的简短字符串。

## 示例

展示如何使用资源 ToString 方法。

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// 打印资源的常规信息
Console.WriteLine(resource.ToString());
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


