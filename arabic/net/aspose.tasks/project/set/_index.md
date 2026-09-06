---
title: "Project.Set"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية"
type: docs
weight: 1240
url: /ar/net/aspose.tasks/project/set/
---
## Set&lt;T&gt;(Key&lt;T, PrjKey&gt;, T) {#set_1}

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set<T>(Key<T, PrjKey> key, T val)
```

| معامل | الوصف |
| --- | --- |
| T | نوع القيمة المرتبطة. |
| key | مفتاح الخاصية المحددة. [`Prj`](../../prj/) للحصول على مفتاح الخاصية. |
| القيمة | القيمة. |

## الأمثلة

يعرض كيفية تعيين سمات المهمة.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Set(Key&lt;DateTime, PrjKey&gt;, DateTime) {#set}

يربط الخاصية المحددة بالقيمة المحددة في هذه الحاوية.

```csharp
public void Set(Key<DateTime, PrjKey> key, DateTime val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| key | Key`2 | مفتاح الخاصية المحددة. [`Prj`](../../prj/) للحصول على مفتاح الخاصية. |
| القيمة | DateTime | القيمة. |

## الأمثلة

يعرض كيفية تعيين سمات المهمة.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


