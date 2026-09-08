---
title: "Not1.Check"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Not 메서드. 지정된 객체가 조건을 만족하면 true를 반환합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

지정된 객체가 조건을 만족하면 true를 반환합니다.

```csharp
public bool Check(T el)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | T | 검사할 객체. |

### 반환 값

객체가 조건을 만족하면 true.

## 예제

&lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt; 조건을 사용하는 방법을 보여줍니다.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 모든 프로젝트 작업을 수집합니다
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // 필터 조건을 생성합니다
    var filter = new NullCondition();

    // 그리고 <see cref=\"Aspose.Tasks.Util.Not`1\" /> 조건을 적용하여 반전합니다
    var condition = new Not<Task>(filter);

    // 수집된 작업에 조건을 적용합니다
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### 또 보기

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


