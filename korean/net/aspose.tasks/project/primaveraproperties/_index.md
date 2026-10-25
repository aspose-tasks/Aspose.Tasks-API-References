---
title: "Project.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. Primavera 파일에서 읽은 프로젝트에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다."
type: docs
weight: 720
url: /ko/net/aspose.tasks/project/primaveraproperties/
---
## Project.PrimaveraProperties property

Primavera 파일에서 읽은 프로젝트에 대한 Primavera 전용 속성을 포함하는 객체를 가져옵니다.

```csharp
public PrimaveraProjectProperties PrimaveraProperties { get; }
```

## 예제

Primavera 파일에서 프로젝트를 읽고 프로젝트의 Primavera 전용 속성을 검사하는 방법을 보여줍니다.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 특수 UID를 가진 프로젝트를 반환합니다.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

// 프로젝트의 일정 옵션이 기본값인 경우 PrimaveraProperties는 null일 수 있습니다.
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

### 또 보기

* class [PrimaveraProjectProperties](../../primaveraprojectproperties/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


