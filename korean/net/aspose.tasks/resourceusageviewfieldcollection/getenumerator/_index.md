---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceUsageViewFieldCollection 메서드. 이 컬렉션에 대한 열거자를 반환합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

이 컬렉션에 대한 열거자를 반환합니다.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### 반환 값

이 컬렉션에 대한 열거자.

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


