---
title: "ExtendedAttribute.FlagValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. 플래그 유형의 속성에 플래그가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

'Flag' 유형을 가진 속성에 플래그가 설정되었는지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool FlagValue { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | [`AttributeDefinition`](../attributedefinition/) 속성이 초기화되지 않았거나 현재 속성이 플래그 속성이 아닌 경우 발생합니다. |

## 예제

불리언 확장 속성을 만드는 방법을 보여줍니다.

```csharp
var project = new Project();

// 새 작업 확장 속성 정의를 생성합니다
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// 속성에 수식을 추가합니다.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// 확장 속성을 생성합니다.
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### 또 보기

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


