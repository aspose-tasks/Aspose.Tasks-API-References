---
title: "ViewCollection.Contains"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ViewCollection 메서드. 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/viewcollection/contains/
---
## ViewCollection.Contains method

지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

```csharp
public bool Contains(View item)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 항목 | View | 찾을 지정된 항목. |

### 반환 값

지정된 항목이 이 컬렉션에 있으면 true; 그렇지 않으면 false.

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


