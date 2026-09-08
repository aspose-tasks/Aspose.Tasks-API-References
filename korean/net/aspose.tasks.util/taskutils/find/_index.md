---
title: "TaskUtils.Find"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskUtils 메서드. 작업 트리에서 조건을 만족하는 작업을 찾습니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

작업 트리에서 조건을 만족하는 작업을 찾습니다.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| root | 작업 | 트리의 루트. |
| cond | ICondition`1 | 적용된 조건. |

### 반환 값

Task가 발견되면 해당 작업, 그렇지 않으면 null.

## 예제

&lt;see cref=\"Aspose.Tasks.Util.TaskUtils.Find\" /&gt; 메서드 사용 방법을 보여줍니다.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 조건을 만족하는 작업의 새 트리를 생성합니다 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// 지정된 객체가 조건을 만족하면 true를 반환합니다.
    /// </summary>
    /// <param name=\"el\">확인할 객체입니다.</param>
    /// <returns>객체가 조건을 만족하면 true를 반환합니다.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


