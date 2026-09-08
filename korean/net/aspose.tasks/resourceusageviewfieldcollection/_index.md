---
title: "클래스 ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection 클래스. ResourceUsageViewField 값들의 컬렉션을 나타냅니다."
type: docs
weight: 1830
url: /ko/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

[`ResourceUsageViewField`](../resourceusageviewfield/) 값들의 컬렉션을 나타냅니다.

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | `ResourceUsageViewFieldCollection` 클래스의 인스턴스를 [`ResourceUsageViewField`](../resourceusageviewfield/) 클래스 인스턴스를 포함하는 리스트로 변환합니다. |

## 예제

ResourceUsageView 인스턴스의 필드 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// 컬렉션을 ResourceUsageViewField 리스트로 변환할 수 있습니다.
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### 또 보기

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


