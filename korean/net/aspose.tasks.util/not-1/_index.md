---
title: "클래스 NotT"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.Not1T 클래스. 지정된 조건에 논리 NOT를 적용합니다"
type: docs
weight: 2750
url: /ko/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

지정된 조건에 논리 NOT을 적용합니다.

```csharp
public class Not<T> : ICondition<T>
```

| 매개변수 | 설명 |
| --- | --- |
| T | 메서드 인터페이스를 적용할 객체 유형. |

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | `Not` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | 지정된 객체가 조건을 만족하면 true를 반환합니다. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


