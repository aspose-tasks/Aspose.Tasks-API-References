---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. Text 유형 속성의 값을 가져오거나 설정합니다"
type: docs
weight: 80
url: /ko/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

'Text' 유형을 가진 속성의 값을 가져오거나 설정합니다.

```csharp
public string TextValue { get; set; }
```

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | [`AttributeDefinition`](../attributedefinition/) 속성이 초기화되지 않았거나 현재 속성이 텍스트 속성이 아닌 경우 발생합니다. |

## 예제

MS Project 날짜/시간 수식을 사용하는 확장 속성을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// ProjDateDiff 수식을 설정하고 확장 속성 값을 출력합니다
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// ProjDateSub 수식을 설정하고 확장 속성 값을 출력합니다
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// 우리는 ProjDurConv 수식을 기간 값 속성뿐만 아니라 텍스트 값 속성에도 설정할 수 있습니다.
// 기간 값 확장 속성에 ProjDurConv 수식을 설정하고 그 값을 출력합니다.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// 텍스트 값 확장 속성에 ProjDurConv 수식을 설정하고 그 값을 출력합니다.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Second 수식을 설정하고 확장 속성 값을 출력합니다
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Weekday 수식을 설정하고 확장 속성 값을 출력합니다
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### 또 보기

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


