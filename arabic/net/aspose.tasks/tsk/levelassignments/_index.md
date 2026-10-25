---
title: "Tsk.LevelAssignments"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كانت وظيفة التوازن يمكنها تأخير وتقسيم التعيينات الفردية لحل الإفراط في التخصيص"
type: docs
weight: 750
url: /ar/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

يحدد ما إذا كانت وظيفة التسوية يمكنها تأخير وتقسيم المهام الفردية من أجل حل التخصيصات الزائدة.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


