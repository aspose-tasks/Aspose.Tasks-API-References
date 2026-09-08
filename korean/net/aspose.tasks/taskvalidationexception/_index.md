---
title: "클래스 TaskValidationException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskValidationException 클래스. 재계산 후 프로젝트 작업에서 오류가 발견될 때 발생하는 예외를 나타냅니다."
type: docs
weight: 2510
url: /ko/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

재계산 후 프로젝트 작업에서 오류가 발견될 때 발생하는 예외를 나타냅니다.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | 예외를 발생시킨 작업을 가져옵니다. |

## 예제

예외가 발생할 수 있는 조건을 보여줍니다 &lt;see cref="TaskValidationException" /&gt; 예외가 발생합니다.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // 실수로 잘못된 날짜를 설정했습니다
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // 검증을 실행하는 플래그와 함께 프로젝트 재계산을 실행합니다
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### 또 보기

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


