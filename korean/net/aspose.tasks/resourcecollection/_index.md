---
title: "클래스 ResourceCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ResourceCollection 클래스. Resource 객체의 컬렉션을 나타냅니다."
type: docs
weight: 1770
url: /ko/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

[`Resource`](../resource/) 객체의 컬렉션을 나타냅니다.

```csharp
public class ResourceCollection : IList<Resource>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | ResourceCollection에 포함된 요소 수를 가져옵니다. 읽기 전용 Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | ResourceCollection 객체의 상위 프로젝트를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | 프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | 프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | 프로젝트 리소스 컬렉션의 지정된 위치에 새 리소스를 추가합니다. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | 직접 삭제는 지원되지 않으며, 이 메서드는 NotSupportedException을 발생시킵니다. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | 지정된 id를 가진 리소스를 반환합니다. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | 지정된 Uid를 가진 리소스를 반환합니다. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | ICollection의 Remove 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | ResourceCollection 객체를 [`Resource`](../resource/) 객체 목록으로 변환합니다. |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


