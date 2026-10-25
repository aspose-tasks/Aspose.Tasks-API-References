---
title: "클래스 TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskUsageViewFieldCollection 클래스. TaskUsageViewField 값들의 컬렉션을 나타냅니다."
type: docs
weight: 2500
url: /ko/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

[`TaskUsageViewField`](../taskusageviewfield/) 값들의 컬렉션을 나타냅니다.

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | 이 컬렉션의 모든 항목을 포함하는 리스트를 반환합니다. |

## 예제

TaskUsageView 인스턴스의 필드 컬렉션을 작업하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// 컬렉션을 TaskUsageViewField 리스트로 변환할 수 있습니다.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### 또 보기

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


