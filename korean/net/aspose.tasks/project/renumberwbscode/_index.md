---
title: "Project.RenumberWBSCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 메서드. 모든 작업의 WBS 코드를 재번호 매깁니다."
type: docs
weight: 1180
url: /ko/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

모든 작업의 WBS 코드를 다시 번호 매깁니다.

```csharp
public void RenumberWBSCode()
```

## 예제

작업의 WBS 코드를 재번호 매기는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// 출력: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// 출력: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### 또 보기

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

통과된 작업의 WBS 코드를 다시 번호 매깁니다.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskIds | List`1 | WBS 코드를 재번호 매기기 위한 작업 식별자. |

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

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


