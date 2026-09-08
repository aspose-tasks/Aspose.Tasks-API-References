---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceUsageViewFieldCollection 메서드. ResourceUsageViewFieldCollection 클래스의 인스턴스를 ResourceUsageViewField 클래스의 인스턴스를 포함하는 리스트로 변환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

[`ResourceUsageViewFieldCollection`](../) 클래스의 인스턴스를 [`ResourceUsageViewField`](../../resourceusageviewfield/) 클래스의 인스턴스를 포함하는 리스트로 변환합니다.

```csharp
public IList<ResourceUsageViewField> ToList()
```

### 반환 값

[`ResourceUsageViewFieldCollection`](../) 클래스의 인스턴스가 [`ResourceUsageViewField`](../../resourceusageviewfield/) 클래스의 인스턴스를 포함하는 리스트로 변환되었습니다.

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

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


