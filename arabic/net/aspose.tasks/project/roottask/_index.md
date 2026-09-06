---
title: "Project.RootTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على جذر شجرة المهام"
type: docs
weight: 800
url: /ar/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

يحصل على جذر شجرة المهام.

```csharp
public Task RootTask { get; }
```

## الأمثلة

يعرض كيفية إضافة مهمة إلى مشروع باستخدام مهمة الجذر للمشروع.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


