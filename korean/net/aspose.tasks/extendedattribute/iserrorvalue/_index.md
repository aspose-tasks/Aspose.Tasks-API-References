---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. 확장 속성 값 계산이 오류로 끝났는지 여부를 가져옵니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

확장 속성 값 계산이 오류를 발생했는지 여부를 가져옵니다.

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


