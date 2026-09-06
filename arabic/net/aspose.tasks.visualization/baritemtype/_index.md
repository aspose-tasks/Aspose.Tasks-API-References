---
title: "تعداد BarItemType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.Visualization.BarItemType. نوع العنصر لتغيير نمط الشريط لـ"
type: docs
weight: 2940
url: /ar/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

نوع العنصر لتغيير نمط الشريط لـ.

```csharp
public enum BarItemType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Task | `0` | يشير إلى نوع عنصر شريط المهمة. |
| Summary | `1` | يشير إلى نوع عنصر شريط الملخص. |
| ProjectSummary | `2` | يشير إلى نوع عنصر شريط ملخص المشروع. |
| ManualTask | `3` | يشير إلى نوع عنصر شريط المهمة اليدوية. |
| InactiveTask | `4` | يشير إلى نوع عنصر شريط المهمة غير النشطة. |
| CriticalTask | `5` | يشير إلى نوع عنصر شريط المهمة الحرجة. |
| Milestone | `6` | يشير إلى نوع عنصر شريط مهمة المعلم. |
| ManualSummary | `7` | يشير إلى نوع عنصر شريط الملخص اليدوي. |
| Split | `8` | يشير إلى نوع عنصر شريط الانقسام. |
| ExternalTasks | `9` | يشير إلى نوع عنصر شريط المهام الخارجية. |
| ExternalMilestone | `10` | يشير إلى نوع عنصر شريط معلم خارجي. |
| Deadline | `11` | يشير إلى نوع عنصر شريط الموعد النهائي. |
| Progress | `12` | يشير إلى نوع عنصر شريط التقدم. |
| StartOnly | `13` | يشير إلى نوع عنصر شريط يبدأ فقط. |
| FinishOnly | `14` | يشير إلى نوع عنصر شريط ينتهي فقط. |
| DurationOnly | `15` | يشير إلى نوع عنصر شريط المدة فقط. |
| InactiveMilestone | `16` | يشير إلى نوع عنصر شريط معلم غير نشط. |
| InactiveSummary | `17` | يشير إلى نوع عنصر شريط ملخص غير نشط. |
| SummaryRollup | `18` | نوع عنصر شريط تجميع الملخص. |

## الأمثلة

يوضح كيفية تخصيص أشرطة المهام باستخدام &lt;see cref="Aspose.Tasks.Visualization.BarStyle" /&gt;s.

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### انظر أيضًا

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


