---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceUsageView 속성. 이 ResourceUsageView의 ResourceUsageViewFieldCollection 객체를 가져옵니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

이 ResourceUsageView의 [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) 객체를 가져옵니다.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## 예제

리소스 사용 보기 필드를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### 또 보기

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


