---
title: "Project.Set"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。将指定属性映射到此容器中的指定值。"
type: docs
weight: 1240
url: /zh/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

将指定属性映射到此容器中的指定值。

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| 参数 | 描述 |
| --- | --- |
| T | 映射值的类型。 |
| key | 指定的属性键。[`Prj`](../../prj/) 用于获取属性键。 |
| val | 该值。 |

## 示例

展示如何设置任务的属性。

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

将指定属性映射到此容器中的指定值。

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | Key`2 | 指定的属性键。[`Prj`](../../prj/) 用于获取属性键。 |
| val | DateTime | 该值。 |

## 示例

展示如何设置任务的属性。

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


