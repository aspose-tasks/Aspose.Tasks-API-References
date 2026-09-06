---
title: "Tsk.DisplayOnTimeline"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يحدد ما إذا كان يجب عرض المهمة في عرض المخطط الزمني"
type: docs
weight: 290
url: /ar/net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

يحدد ما إذا كان يجب عرض المهمة في عرض الخط الزمني.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Tsk.DisplayOnTimeline.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


