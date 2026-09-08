---
title: "Project.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 루트 작업의 모든 하위 작업을 재귀적으로 수집합니다."
type: docs
weight: 1230
url: /ko/net/aspose.tasks/project/selectallchildtasks/
---
## Project.SelectAllChildTasks method

루트 작업의 모든 하위 작업을 재귀적으로 수집합니다.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### 반환 값

작업 컬렉션.

## 예제

선택된 작업의 WBS 코드를 재번호 매기는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// 출력: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// 출력: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### 또 보기

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


