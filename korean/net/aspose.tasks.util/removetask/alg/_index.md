---
title: "RemoveTask.Alg"
second_title: "Aspose.Tasks for .NET API 참조"
description: "RemoveTask 메서드. 아무 작업도 수행하지 않습니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/removetask/alg/
---
## RemoveTask.Alg method

아무 것도 하지 않습니다.

```csharp
public void Alg(Task el, int level)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | 작업 | 처리할 객체. |
| 레벨 | Int32 | 트리 노드 레벨. |

## 예제

&lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt; 트리 기반 알고리즘 사용 방법을 보여줍니다.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // 트리 기반 알고리즘을 사용하여 트리에서 task1을 삭제합니다.
    var algorithm = new RemoveTask(task1);

    // 알고리즘을 작업 트리에 적용합니다.
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // 결과를 확인합니다.
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


