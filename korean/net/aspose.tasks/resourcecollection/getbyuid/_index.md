---
title: "ResourceCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceCollection 메서드. 지정된 Uid를 가진 리소스를 반환합니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks/resourcecollection/getbyuid/
---
## ResourceCollection.GetByUid method

지정된 Uid를 가진 리소스를 반환합니다.

```csharp
public Resource GetByUid(int uid)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | Int32 | 지정된 uid. |

### 반환 값

지정된 uid를 가진 리소스가 있으면 반환하고, 없으면 null을 반환합니다.

## 비고

O(1) 복잡도.

## 예제

리소스 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// 빈 리소스를 추가합니다
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// 이름이 있는 리소스를 추가합니다
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// 지정된 ID를 가진 리소스 앞에 리소스를 추가합니다
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// id로 리소스를 가져옵니다
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// 리소스 컬렉션은 Clear 작업을 지원하지 않습니다
// project.Resources.Clear();
// 다음 코드 샘플을 대신 사용하십시오
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### 또 보기

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


