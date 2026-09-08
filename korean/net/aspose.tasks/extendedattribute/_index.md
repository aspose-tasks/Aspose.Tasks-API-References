---
title: "클래스 ExtendedAttribute"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ExtendedAttribute 클래스. 확장 속성을 나타냅니다"
type: docs
weight: 520
url: /ko/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

확장 속성을 나타냅니다.

```csharp
public class ExtendedAttribute
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | 속성 정의를 가져옵니다. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | 날짜 유형(Date, Start, Finish)을 가진 속성의 값을 가져오거나 설정합니다. |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | 'Duration' 유형을 가진 속성의 값을 가져오거나 설정합니다. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | 필드의 ID를 가져옵니다. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | 'Flag' 유형을 가진 속성에 플래그가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | 확장 속성 값 계산이 오류를 발생했는지 여부를 가져옵니다. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | 숫자 유형(Cost, Number)을 가진 속성의 값을 가져오거나 설정합니다. |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | 'Text' 유형을 가진 속성의 값을 가져오거나 설정합니다. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | 조회 값의 GUID를 가져옵니다. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | 이 `ExtendedAttribute` 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. 이 개체에 대해 [`ExtendedAttributeDefinition`](../extendedattributedefinition/)에 수식이나 롤업이 정의되어 있으면 true를 반환합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | 확장 속성의 짧은 문자열 표현을 반환합니다. |

## 비고

현재 MSP Xml 2003/2007 및 mpp 2003에서 확장 속성을 읽는 모든 유형을 지원합니다. MSP mpp 2007의 경우, 지속 시간과 플래그를 제외한 모든 확장 속성 읽기를 지원합니다.

## 예제

사용자가 지정한 수식을 사용하여 값이 계산되는 사용자 정의 필드를 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 확장 속성 정의를 생성합니다
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// 속성에 수식을 추가합니다.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// 확장 속성 만들기
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// 확장 속성에 수식을 설정했으므로 읽기 전용입니다(값이 수식을 사용하여 계산됩니다).
// 출력은 "Value is read only" 입니다
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// 읽기 전용 필드의 값을 설정하려고 시도할 수 있지만 효과가 없습니다.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


