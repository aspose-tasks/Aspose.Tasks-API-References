---
title: "VbaModuleAttribute.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModuleAttribute 方法。返回一个值，指示此实例是否等于指定的 VbaModuleAttribute 对象"
type: docs
weight: 30
url: /zh/net/aspose.tasks/vbamoduleattribute/equals/
---
## Equals(VbaModuleAttribute) {#equals}

返回一个值，指示此实例是否等于指定的 [`VbaModuleAttribute`](../) 对象。

```csharp
public bool Equals(VbaModuleAttribute other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | VbaModuleAttribute | 要与此实例比较的指定 [`VbaModuleAttribute`](../) 对象。 |

### 返回值

如果此实例等于指定的 [`VbaModuleAttribute`](../) 对象，则返回 true；否则返回 false。

## 示例

展示如何检查 VBA 模块属性的相等性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### 另见

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的 [`VbaModuleAttribute`](../) 对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | Object | 要与此实例比较的指定 [`VbaModuleAttribute`](../) 对象。 |

### 返回值

如果此实例等于指定的 [`VbaModuleAttribute`](../) 对象，则返回 true；否则返回 false。

## 示例

展示如何检查 VBA 模块属性的相等性。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];
Console.WriteLine("Module attribute 1 Key: {0}, Value: {1}", attribute1.Key, attribute1.Value);
Console.WriteLine("Module attribute 2 Key: {0}, Value: {1}", attribute2.Key, attribute2.Value);
Console.WriteLine("Are module attributes equal: " + attribute1.Equals(attribute2));
```

### 另见

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


