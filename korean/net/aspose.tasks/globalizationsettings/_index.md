---
title: "클래스 GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.GlobalizationSettings 클래스. 프로젝트의 글로벌화 설정을 나타냅니다."
type: docs
weight: 720
url: /ko/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

프로젝트의 글로벌화 설정을 나타냅니다.

```csharp
public class GlobalizationSettings
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | 수식에서 사용되는 부울 'false' 리터럴에 대한 문자열을 가져옵니다. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | 날짜 필드에 대한 수식에서 사용되는 "NA"(빈 값) 리터럴을 가져옵니다. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | 수식에서 사용되는 부울 'true' 리터럴에 대한 문자열을 가져옵니다. |

## 비고

권장되는 방법은 프로젝트 전체에서 문화에 독립적인 리터럴이나 형식을 사용하는 것입니다. 그러나 프로젝트가 문화별 리터럴을 사용하는 경우, 이 클래스를 사용하여 수식 계산 엔진이 해당 리터럴을 구문 분석하도록 도울 수 있습니다.

## 예제

프로젝트의 언어별 설정을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// 확장 속성 만들기
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


