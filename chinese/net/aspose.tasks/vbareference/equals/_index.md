---
title: "VbaReference.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaReference 方法。返回一个值，指示此实例是否等于指定的 VbaReference 对象"
type: docs
weight: 40
url: /zh/net/aspose.tasks/vbareference/equals/
---
## Equals(VbaReference) {#equals}

返回一个值，指示此实例是否等于指定的 [`VbaReference`](../) 对象。

```csharp
public bool Equals(VbaReference other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | VbaReference | 用于与此实例比较的指定 [`VbaReference`](../) 对象。 |

### 返回值

如果此实例等于指定的 [`VbaReference`](../) 对象，则返回 true；否则返回 false。

## 示例

展示如何检查 VBA 引用的相等性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 引用的相等性是根据引用的名称进行检查的。
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### 另见

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的 [`VbaReference`](../) 对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | Object | 用于与此实例比较的指定 [`VbaReference`](../) 对象。 |

### 返回值

如果此实例等于指定的 [`VbaReference`](../) 对象，则返回 true；否则返回 false。

## 示例

展示如何检查 VBA 引用的相等性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// 引用的相等性是根据引用的名称进行检查的。
Console.WriteLine("VBA reference 1 Name: " + reference1.Name);
Console.WriteLine("VBA reference 2 Name: " + reference2.Name);
Console.WriteLine("Are references equal: " + reference1.Equals(reference2));
```

### 另见

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


