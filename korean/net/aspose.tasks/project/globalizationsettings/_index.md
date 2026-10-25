---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트의 지역화 언어별 설정을 가져오거나 설정합니다."
type: docs
weight: 460
url: /ko/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

프로젝트의 글로벌화(언어별) 설정을 가져오거나 설정합니다.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## 비고

권장되는 방법은 프로젝트 전체에서 문화에 의존하지 않는 리터럴이나 형식을 사용하는 것입니다. 그러나 프로젝트가 문화에 특화된 리터럴을 사용하는 경우, 이 클래스를 사용하여 계산 엔진이 해당 리터럴을 파싱하도록 도울 수 있습니다.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


