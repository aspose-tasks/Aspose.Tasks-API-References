---
title: "Tsk.Duration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. المدة الإجمالية لوقت العمل النشط للمهمة كما تم إدخاله أو كما يحسبه Microsoft Project بناءً على تاريخ البدء وتاريخ الانتهاء والتقويمات وعوامل الجدولة الأخرى."
type: docs
weight: 300
url: /ar/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

الفترة الإجمالية للوقت النشط للعمل للمهمة كما تم إدخالها أو كما تم حسابها بواسطة Microsoft Project بناءً على تاريخ البدء، تاريخ الانتهاء، الجداول الزمنية، وعوامل الجدولة الأخرى.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## الأمثلة

يعرض كيفية تعيين مدة المهمة.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


