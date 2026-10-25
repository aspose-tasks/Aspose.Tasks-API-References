---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskUsageView 속성. 이 TaskUsageView의 TaskUsageViewFieldCollection 객체를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

이 TaskUsageView의 [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) 객체를 가져옵니다.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## 예제

작업 사용 보기 필드를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### 또 보기

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


