---
title: "Resource.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 方法。返回一个值，指示此实例是否等于 Resource 类的指定实例。"
type: docs
weight: 820
url: /zh/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

返回一个值，指示此实例是否等于 [`Resource`](../) 类的指定实例。

```csharp
public bool Equals(Resource other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | Resource | 用于与此实例比较的 [`Resource`](../) 类的指定实例。 |

### 返回值

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## 示例

展示如何检查资源相等性。

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 与此实例比较的对象。 |

### 返回值

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## 示例

展示如何检查资源相等性。

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


