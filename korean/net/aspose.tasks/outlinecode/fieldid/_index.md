---
title: "OutlineCode.FieldId"
second_title: "Aspose.Tasks for .NET API 참조"
description: "OutlineCode 속성. 프로젝트 Id 사용자 정의 필드의 숫자 값을 가져오거나 설정합니다"
type: docs
weight: 20
url: /ko/net/aspose.tasks/outlinecode/fieldid/
---
## OutlineCode.FieldId property

프로젝트 Id 사용자 정의 필드의 숫자 값을 가져오거나 설정합니다.

```csharp
public string FieldId { get; set; }
```

## 예제

작업의 개요 코드를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// 개요 코드 읽기
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### 또 보기

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


