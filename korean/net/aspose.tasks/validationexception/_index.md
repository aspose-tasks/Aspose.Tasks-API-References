---
title: "클래스 ValidationException"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ValidationException 클래스. 엔터티 검증 중 오류가 발견될 때 발생하는 예외를 나타냅니다."
type: docs
weight: 2790
url: /ko/net/aspose.tasks/validationexception/
---
## ValidationException class

엔터티 검증 중 오류가 발견될 때 발생하는 예외를 나타냅니다.

```csharp
public class ValidationException : ApplicationException
```

## 예제

반복 작업을 작업할 때 &lt;see cref=\"ValidationException\"/&gt;을 처리하는 방법을 보여줍니다.

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


