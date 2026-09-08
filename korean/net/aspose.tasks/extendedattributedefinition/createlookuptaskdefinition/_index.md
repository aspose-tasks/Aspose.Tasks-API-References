---
title: "ExtendedAttributeDefinition.CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. 조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 Lookup과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 fieldId와 alias를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](../calculationtype/)이 Lookup과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *fieldId*와 *alias*를 지정해야 합니다. 필드 유형은 field id에서 추론됩니다.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | 지정된 [`ExtendedAttributeTask`](../../extendedattributetask/) 필드 ID. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *fieldId*와 *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 조회가 포함된 작업용 사용자 정의 필드 정의를 만든 다음 텍스트 값으로 채우세요:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

업데이트된 확장 속성 정의를 작성하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// lookup과 하나의 lookup 값을 가진 새로운 text3 확장 속성을 추가합니다
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// lookup과 두 개의 비용 값을 가진 새로운 cost1 확장 속성을 추가합니다
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// 새 작업을 추가하고 속성 lookup 값을 할당합니다.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// lookup 없이 기간 속성을 정의합니다.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// 새 작업을 추가하고 이전에 정의된 기간 속성에 기간 값을 할당합니다.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### 또 보기

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

조회가 포함된 확장 속성 정의를 생성하는 팩터리 메서드입니다. [`CalculationType`](../calculationtype/)이 Lookup과 같으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *customFieldType*, *fieldId* 및 *alias*를 지정해야 합니다.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 지정된 [`CustomFieldType`](../../customfieldtype/) 유형입니다. |
| fieldId | ExtendedAttributeTask | 지정된 [`ExtendedAttributeTask`](../../extendedattributetask/) 필드 ID. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *customFieldType*, *fieldId*, *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 조회가 포함된 작업용 사용자 정의 필드 정의를 만든 다음 텍스트 값으로 채우세요:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
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

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


