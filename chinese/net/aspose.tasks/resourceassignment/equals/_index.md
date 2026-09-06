---
title: "ResourceAssignment.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。返回一个值，指示此实例是否等于指定的 ResourceAssignment 类实例"
type: docs
weight: 690
url: /zh/net/aspose.tasks/resourceassignment/equals/
---
## Equals(ResourceAssignment) {#equals}

返回一个值，指示此实例是否等于 [`ResourceAssignment`](../) 类的指定实例。

```csharp
public bool Equals(ResourceAssignment other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | ResourceAssignment | 用于与此实例比较的 [`ResourceAssignment`](../) 类的指定实例。 |

### 返回值

**True** if the specified instance of the [`ResourceAssignment`](../) class has the same UID value as this instance; otherwise, **false**.

## 示例

展示如何检查资源分配的相等性。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### 另见

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
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

**True** if o is a ResourceAssignment that assign the same resource and task as this instance; otherwise, **false**.

## 示例

展示如何检查资源分配的相等性。

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(1);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(1);

Console.WriteLine("Are resource assignments equal: " + resourceAssignment1.Equals(resourceAssignment2));
```

### 另见

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


