---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. 내부 조회 목록에 값을 추가합니다. 이는 ValueList를 조작하는 권장 방법입니다."
type: docs
weight: 300
url: /ko/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

내부 조회 목록에 값을 추가합니다. 이는 [`ValueList`](../valuelist/)를 조작하는 권장 방법입니다.

```csharp
public void AddLookupValue(Value value)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | 값 | 조회에 추가할 값. |

## 비고

이 메서드는 [`ExtendedAttributeDefinition`](../) 인스턴스 중에서 [`CalculationType`](../calculationtype/)이 Lookup인 경우에만 작동합니다.

## 예제

이 코드를 사용하여 조회 목록에 새 값을 추가하세요:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

할당에 대한 조회가 포함된 확장 속성을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 리소스 "1 TRG: Trade Group"을 "TASK 1"에 ResourceAssignment 객체를 생성하여 할당합니다.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// 조회가 포함된 사용자 정의 속성 정의를 생성합니다.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// 이 값은 MS Project의 "Resource usage" 보기에서 확인할 수 있습니다.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// 조회가 포함된 사용자 정의 속성 정의를 생성합니다.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// 이 값은 MS Project의 "Task usage" 보기에서 확인할 수 있습니다.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// 잘못된 값은 나중에 제거될 수 있습니다.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// 프로젝트 작업 중...
```

### 또 보기

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


