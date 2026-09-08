---
title: "PrimaveraProjectProperties.BaselineProjects"
second_title: "Aspose.Tasks for .NET API 참조"
description: "PrimaveraProjectProperties 속성. 현재 프로젝트의 기준선 프로젝트 배열을 가져옵니다. 내보낸 기준선을 포함하는 Primavera XML 파일에서 읽은 프로젝트에 적용됩니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/primaveraprojectproperties/baselineprojects/
---
## PrimaveraProjectProperties.BaselineProjects property

중요 활동을 정의하는 방법을 가져옵니다: 최장 경로 또는 총 부동(Total Float) 접근법.

```csharp
public Project[] BaselineProjects { get; }
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

* class [Project](../../project/)
* class [PrimaveraProjectProperties](../)
* namespace [Aspose.Tasks](../../primaveraprojectproperties/)
* assembly [Aspose.Tasks](../../../)


