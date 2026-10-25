---
title: "And1.And"
second_title: "Aspose.Tasks for .NET API 참조"
description: "And 생성자. And 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

[`And`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| cond1 | ICondition`1 | 첫 번째 조건. |
| cond2 | ICondition`1 | 두 번째 조건. |

## 예제

&lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt; 조건을 사용하는 방법을 보여줍니다.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 모든 프로젝트 작업을 수집합니다
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // 요약 작업을 필터링하는 필터 조건을 생성합니다
    var condition1 = new SummaryCondition();

    // null이 아닌 작업을 필터링하는 필터 조건을 생성합니다
    var condition2 = new NotNullCondition();

    // 그리고 <see cref=\"Aspose.Tasks.Util.And`1\" /> 조건을 적용하여 결합합니다
    var joinedCondition = new And<Task>(condition1, condition2);

    // 수집된 작업에 조건을 적용합니다
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

        // 다른 속성과 함께 작업합니다...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### 또 보기

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


