---
title: "클래스 ViewCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ViewCollection 클래스. View 객체 목록을 포함합니다. ICollectionView 인터페이스를 구현합니다."
type: docs
weight: 2900
url: /ko/net/aspose.tasks/viewcollection/
---
## ViewCollection class

[`View`](../view/) 객체 목록을 포함합니다. ICollection&lt;View&gt; 인터페이스를 구현합니다.

```csharp
public class ViewCollection : ICollection<View>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | View 객체의 상위 항목을 가져옵니다. 읽기 전용 [`Project`](../project/). |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | 이름이 일치하는 View를 검색하고, 컬렉션 내 첫 번째 항목을 반환합니다. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | 지정된 Screen 속성을 가진 View를 검색하고, 컬렉션 내 첫 번째 항목을 반환합니다. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | view 컬렉션을 [`View`](../view/) 객체 목록으로 변환합니다. |

## 예제

view 컬렉션 작업 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// view를 일반 목록으로 변환
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// 새 view 추가
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// view를 반복
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// view를 한 번에 모두 제거
project.Views.Clear();

// 또는 하나씩
{
    // 방법 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // 방법 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### 또 보기

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


