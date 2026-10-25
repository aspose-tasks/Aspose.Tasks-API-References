---
title: "클래스 OutlineCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.OutlineCode 클래스. 개요 코드의 값을 나타냅니다"
type: docs
weight: 1150
url: /ko/net/aspose.tasks/outlinecode/
---
## OutlineCode class

아웃라인 코드의 값을 나타냅니다.

```csharp
public class OutlineCode
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | `OutlineCode` 클래스의 새 인스턴스를 초기화합니다. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | 지정된 개요 코드와 해당 값 중 하나를 사용하여 `OutlineCode` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | 프로젝트 Id 사용자 정의 필드의 숫자 값을 가져오거나 설정합니다. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | 값 목록에 있는 값의 GUID를 가져오거나 설정합니다. ValueGuid는 값 목록의 FieldGuid와 일치합니다. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | 개요 코드 컬렉션의 정의와 연결된 값 목록의 Id를 가져오거나 설정합니다. |

## 비고

두 개의 데이터가 필요합니다 - FieldId로 지정된 개요 코드 테이블에 대한 포인터와 ValueId 또는 ValueGuid 포인터로 지정된 값 목록의 값.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


