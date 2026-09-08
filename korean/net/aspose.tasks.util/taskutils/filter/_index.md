---
title: "TaskUtils.Filter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskUtils 메서드. 조건을 만족하는 작업의 새 트리를 생성합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

조건을 만족하는 작업들의 새로운 트리를 구축합니다.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | 작업 | 트리의 루트. |
| cond | ICondition`1 | 적용된 조건. |

### 반환 값

새 트리의 루트.

## 예제

조건을 사용하는 방법을 보여줍니다.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 조건을 만족하는 작업의 새 트리를 생성합니다 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // 트리에서 작업을 수집합니다
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // 일반 작업 목록을 반복합니다 
    // 기간이 2 작업일 이상인 경우
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// 지정된 객체가 조건을 만족하면 true를 반환합니다.
    /// </summary>
    /// <param name=\"el\">확인할 객체입니다.</param>
    /// <returns>객체가 조건을 만족하면 true를 반환합니다.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


