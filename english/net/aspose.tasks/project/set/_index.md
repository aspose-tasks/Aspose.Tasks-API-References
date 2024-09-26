---
title: Project.Set
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Maps the specified property to the specified value in this container
type: docs
weight: 1240
url: /net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

Maps the specified property to the specified value in this container.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| Parameter | Description |
| --- | --- |
| T | the type of the mapped value. |
| key | the specified property key. [`Prj`](../../prj/) for getting the property key. |
| val | the value. |

## Examples

Shows how to set task's attributes.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

Maps the specified property to the specified value in this container.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| Parameter | Type | Description |
| --- | --- | --- |
| key | Key`2 | the specified property key. [`Prj`](../../prj/) for getting the property key. |
| val | DateTime | the value. |

## Examples

Shows how to set task's attributes.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


