---
title: "ExtendedAttribute.DateValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. 날짜 유형(Date, Start, Finish) 속성의 값을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

날짜 유형(Date, Start, Finish)을 가진 속성의 값을 가져오거나 설정합니다.

```csharp
public DateTime DateValue { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | [`AttributeDefinition`](../attributedefinition/) 속성이 초기화되지 않았거나 현재 속성이 날짜 속성이 아닌 경우 예외가 발생합니다. |

## 예제

확장 속성의 속성 정의를 변경하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 확장 속성 정의를 생성합니다
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// 속성에 수식을 추가합니다.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// 확장 속성을 생성합니다.
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// 새 날짜 확장 속성 정의를 생성합니다
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// 속성에 수식을 추가합니다.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### 또 보기

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


