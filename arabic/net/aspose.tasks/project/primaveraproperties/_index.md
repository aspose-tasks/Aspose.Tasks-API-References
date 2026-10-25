---
title: "Project.PrimaveraProperties"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على كائن يحتوي على خصائص Primaveraspecific لمشروع تم قراءته من ملف Primavera"
type: docs
weight: 720
url: /ar/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

يحصل على كائن يحتوي على خصائص خاصة بـ Primavera لمشروع تم قراءته من ملف Primavera.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## الأمثلة

يعرض كيفية قراءة مشروع من ملف Primavera وفحص خصائص المشروع Primavera-specific.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// يمكن أن تكون PrimaveraProperties فارغة إذا كانت خيارات جدول المشروع لديها القيم الافتراضية.
if (project.PrimaveraProperties != null)
{
    Console.WriteLine("Project's schedule options:");
    Console.WriteLine("Relationship Lag Calendar: " + project.PrimaveraProperties.RelationshipLagCalendar);
    Console.WriteLine("Make Open Ended Activities Critical: " + project.PrimaveraProperties.MakeOpenEndedActivitiesCritical);
    Console.WriteLine("Ignore Other Project Relationships: " + project.PrimaveraProperties.IgnoreOtherProjectRelationships);
    Console.WriteLine("Use Expected Finish Dates: " + project.PrimaveraProperties.UseExpectedFinishDates);

    Console.WriteLine("How critical activities are defined: " +
                      project.PrimaveraProperties.CriticalActivitiesDefiningMethod);

    if (project.PrimaveraProperties.CriticalActivitiesDefiningMethod == PrimaveraCriticalActivitiesDefiningMethod.TotalFloat)
    {
        Console.WriteLine("Total Float threshold for critical activities: " + project.PrimaveraProperties.CriticalTotalFloatLimit);
    }
}
```

### انظر أيضًا

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


