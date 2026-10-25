---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttributeDefinition 메서드. Microsoft Project에서 'None'으로 표시되는 간단한 확장 속성 정의를 생성하는 팩터리 메서드입니다. CalculationType이 None으로 설정되어 있으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 customFieldType, fieldId 및 alias를 지정해야 합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

간단한 확장 속성 정의를 생성하는 팩터리 메서드이며, Microsoft Project에서 "None"으로 표시됩니다. [`CalculationType`](../calculationtype/)이 None으로 설정되어 있으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *customFieldType*, *fieldId*, *alias*를 지정해야 합니다.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| customFieldType | CustomFieldType | 지정된 [`CustomFieldType`](../../customfieldtype/) 유형입니다. |
| fieldId | ExtendedAttributeTask | 지정된 [`ExtendedAttributeTask`](../../extendedattributetask/) 필드 ID. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *customFieldType*, *fieldId*, *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 생성합니다:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

작업의 확장 속성을 만드는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Text1 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// 프로젝트의 확장 속성 컬렉션에 추가합니다.
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// 프로젝트에 작업을 추가합니다.
var task = project.RootTask.Children.Add("Task 1");

// 속성 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// 생성된 확장 속성에 값을 할당합니다. 속성의 유형은 "Text"이며, "TextValue" 속성을 사용해야 합니다.
taskExtendedAttributeText1.TextValue = "London";

// 작업에 확장 속성을 추가합니다.
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Text2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// 확장 속성 정의에 조회 값을 추가합니다.
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// 프로젝트의 확장 속성 컬렉션에 추가합니다.
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// 프로젝트에 작업을 추가합니다.
var task2 = project4.RootTask.Children.Add("Task 2");

// Id 1에 대한 Text2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// 작업에 확장 속성을 추가합니다.
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Duration2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// 확장 속성 정의에 대한 조회 값을 추가합니다.
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// 정의를 프로젝트의 확장 속성 컬렉션에 추가합니다.
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// 프로젝트에 작업을 추가합니다.
var task3 = project2.RootTask.Children.Add("Task 3");

// Id 3에 대한 Duration2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// 작업에 확장 속성을 추가합니다.
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Finish2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// 확장 속성 정의에 대한 조회 값을 추가합니다.
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// 정의를 프로젝트의 확장 속성 컬렉션에 추가합니다.
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// 프로젝트에 작업을 추가합니다.
var task4 = project3.RootTask.Children.Add("Task 4");

// Id 3에 대한 Finish2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// 작업에 확장 속성을 추가합니다.
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

단순한 확장 속성 정의를 생성하는 팩터리 메서드이며, Microsoft Project에서는 "None"으로 표시됩니다. 이 정의는 [`CalculationType`](../calculationtype/)이 None으로 설정되어 있으며 작업에서만 사용할 수 있습니다. 이 메서드를 호출할 때 *fieldId*와 *alias*를 지정해야 합니다. 필드 유형은 필드 ID에서 추론됩니다.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | 지정된 [`ExtendedAttributeTask`](../../extendedattributetask/) 필드 ID. |
| 별칭 | 문자열 | 지정된 문자열 별칭입니다. |

### 반환 값

지정된 *fieldId*와 *alias*를 사용하여 [`ExtendedAttributeDefinition`](../) 클래스의 인스턴스를 생성했습니다.

## 예제

이 예제를 사용하여 사용자 정의 텍스트 필드 정의를 생성합니다:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

확장 속성 정의를 생성하고 구성 중에 속성의 문자열 값을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// 'Common Info'와 동일한 값을 가진 확장 속성을 생성합니다.
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// 'Common Info' 값으로 초기화된 확장 속성을 추가합니다.
task.ExtendedAttributes.Add(extendedAttribute);
```

### 또 보기

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


