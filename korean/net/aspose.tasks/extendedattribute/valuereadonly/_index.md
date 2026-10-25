---
title: "ExtendedAttribute.ValueReadOnly"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. 이 ExtendedAttribute 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. 해당 객체에 대해 ExtendedAttributeDefinition에 수식이나 롤업이 정의되어 있으면 true를 반환합니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/extendedattribute/valuereadonly/
---
## ExtendedAttribute.ValueReadOnly property

이 [`ExtendedAttribute`](../) 인스턴스의 값이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. 해당 객체에 대해 [`ExtendedAttributeDefinition`](../../extendedattributedefinition/)에 수식이나 롤업이 정의되어 있으면 true를 반환합니다.

```csharp
public bool ValueReadOnly { get; }
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


