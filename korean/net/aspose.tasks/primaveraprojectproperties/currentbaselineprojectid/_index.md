---
title: "PrimaveraProjectProperties.CurrentBaselineProjectId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraProjectProperties 속성. 현재 기준선 프로젝트의 Id를 가져옵니다. 내보낸 기준선을 포함하는 Primavera XML 파일에서 읽은 프로젝트에 적용됩니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/primaveraprojectproperties/currentbaselineprojectid/
---
## PrimaveraProjectProperties.CurrentBaselineProjectId property

현재 기준선 프로젝트의 Id를 가져옵니다. 내보낸 기준선을 포함하는 Primavera XML 파일에서 읽은 프로젝트에 적용됩니다.

```csharp
public int CurrentBaselineProjectId { get; }
```

## 예제

Primavera XML 파일에서 프로젝트를 읽고 기준선 프로젝트 데이터를 검사하는 방법을 보여줍니다.

```csharp
Project project = new Project(DataDir + "BaselineProjects.xml");

Console.WriteLine("Current baseline project uid: " + project.PrimaveraProperties.CurrentBaselineProjectId);

foreach (var baselineProject in project.PrimaveraProperties.BaselineProjects)
{
    Console.WriteLine("Baseline project: uid: {0}, name: '{1}'", baselineProject.Uid, baselineProject.Name);
}

var baseline1 = project.PrimaveraProperties.BaselineProjects[1];

var task = GetTaskByActivityId(project, "A1000");
var baselineTask = GetTaskByActivityId(baseline1, "A1000");

Console.WriteLine("Task budgeted total cost: " + task.PrimaveraProperties.BudgetedTotalCost);
Console.WriteLine("Task baseline budgeted total cost: " + baselineTask.PrimaveraProperties.BudgetedTotalCost);
```

### 또 보기

* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


