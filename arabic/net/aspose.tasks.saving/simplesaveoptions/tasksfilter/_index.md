---
title: "SimpleSaveOptions.TasksFilter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SimpleSaveOptions. تحصل أو تعيين الشرط الذي يُستخدم لتصفية المهام المعروضة في ورقة مخطط جانت ومخططات استخدام المهام"
type: docs
weight: 30
url: /ar/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

يحصل أو يعيّن الشرط المستخدم لتصفية المهام المعروضة على مخططات جانت، ورقة المهام، واستخدام المهام.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## ملاحظات

إذا لم يتم تحديد القيمة، يتم استخدام الفلتر الافتراضي الذي يزيل المهام غير المرئية -- أي المهام التابعة للمهام المدمجة.

## الأمثلة

يوضح كيفية استخدام مرشح مهام مخصص أثناء حفظ ملف MS Project.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // قم بتعيين مرشح مهمة لتخطي المهمة 'Task5' و 'Task3'.
        TasksFilter = new CustomTasksFilter()
    };

    // دعنا نتحقق من تنسيق الحفظ.
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // حفظ المشروع كصورة
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// مثال على مرشح مهمة مخصص يمكن استخدامه أثناء حفظ ملف MS Project (على سبيل المثال) بصيغة PDF.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### انظر أيضًا

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


