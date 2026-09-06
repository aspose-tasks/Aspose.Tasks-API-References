---
title: "Project.CalculationMode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل أو تعين وضع الحساب لمشروع. يمكن أن تكون واحدة من قيم تعداد CalculationMode"
type: docs
weight: 110
url: /ar/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

تحصل أو تعين وضع الحساب لمشروع. يمكن أن تكون واحدة من قيم تعداد `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## الأمثلة

يعرض كيفية استخدام وضع حساب المشروع.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// حدد تاريخ بدء المشروع وأضف مهامًا جديدة
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// تم ضبط الخصائص الضرورية في الوضع اليدوي
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// عند ربط مهمتين معًا لا يتم إعادة حساب تواريخهما في الوضع اليدوي
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// لم يتم تغيير بدء المهمة 2
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### انظر أيضًا

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


