---
title: "Task.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 확장 속성의 값을 포함하는 ExtendedAttributeCollection 객체를 가져옵니다."
type: docs
weight: 400
url: /ko/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

확장 속성의 값을 포함하는 ExtendedAttributeCollection 객체를 가져옵니다.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## 비고

두 개의 데이터가 필요합니다 - 고유 ID 또는 필드 ID 중 하나로 지정되는 확장 속성 테이블에 대한 포인터와, 값 자체로 지정되거나 값 목록에 대한 포인터로 지정되는 값.

## 예제

작업 확장 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// 확장 속성 정의 생성
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// 인덱스 0인 작업을 가져옵니다
var tsk = project.RootTask.Children.GetById(1);

// 확장 속성 추가
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// 다음과 같은 짧은 구문도 사용할 수 있습니다: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Text1 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// 프로젝트의 확장 속성 컬렉션에 추가합니다.
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// 속성 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// 생성된 확장 속성에 값을 할당합니다. 속성의 유형은 "Text"이며, "TextValue" 속성을 사용해야 합니다.
taskExtendedAttributeText1.TextValue = "London";

// 작업에 확장 속성을 추가합니다.
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Text2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// 확장 속성 정의에 조회 값을 추가합니다.
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// 프로젝트의 확장 속성 컬렉션에 추가합니다.
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Id 1에 대한 Text2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// 작업에 확장 속성을 추가합니다.
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Duration2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// 확장 속성 정의에 대한 조회 값을 추가합니다.
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// 정의를 프로젝트의 확장 속성 컬렉션에 추가합니다.
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Id 3에 대한 Duration2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// 작업에 확장 속성을 추가합니다.
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Finish2 유형의 확장 속성 정의를 생성합니다.
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// 확장 속성 정의에 대한 조회 값을 추가합니다.
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// 정의를 프로젝트의 확장 속성 컬렉션에 추가합니다.
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Id 3에 대한 Finish2 조회 정의에서 확장 속성을 생성합니다.
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// 작업에 확장 속성을 추가합니다.
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 작업에 대한 확장 속성을 읽습니다.
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### 또 보기

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


