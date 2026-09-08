---
title: "클래스 AndAllConditionT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.AndAllCondition1T 클래스. 모든 조건에 논리 AND를 적용합니다. 예: cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /ko/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

모든 조건에 논리 AND를 적용합니다. 예: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| 매개변수 | 설명 |
| --- | --- |
| T | 메서드 인터페이스를 적용할 객체 유형. |

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | `AndAllCondition` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |

## 예제

&lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt; 조건 사용 방법을 보여줍니다.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // 모든 프로젝트 작업을 수집합니다
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // null이 아닌 작업을 필터링하는 필터 조건을 생성합니다
                             new NotNullCondition(),

                             // 요약 작업을 필터링하는 필터 조건을 생성합니다
                             new SummaryCondition()
                         };

    // 그리고 <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /> 조건을 적용하여 결합합니다.
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // 수집된 작업에 조건을 적용합니다
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


