---
title: "Task.Children"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Task. تحصل على مجموعة مهام فرعية لهذا الكائن. كائن TaskCollection الذي يمثل مهام الأطفال"
type: docs
weight: 190
url: /ar/net/aspose.tasks/task/children/
---
## Task.Children property

يحصل على مجموعة مهام فرعية لهذا الكائن. كائن TaskCollection الذي يمثل المهام الفرعية.

```csharp
public TaskCollection Children { get; }
```

## الأمثلة

يظهر كيفية استخدام مجموعة المهام لإضافة مهمة.

```csharp
var project = new Project();

// إضافة مهمة، مهمة فرعية وحفظ المشروع
var task = project.RootTask.Children.Add("Summary1");
task.Children.Add("Subtask1");
project.Save(OutDir + "CreateTasks_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


