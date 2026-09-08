---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 속성. 이 객체에 대한 ExtendedAttributeCollection 클래스의 인스턴스를 가져오거나 설정합니다."
type: docs
weight: 250
url: /ko/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

이 개체에 대한 ExtendedAttributeCollection 클래스의 인스턴스를 가져오거나 설정합니다.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## 비고

XML 형식에 대해서만 읽기가 지원됩니다.

## 예제

할당에 대한 확장 속성을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// 리소스 "1 TRG: Trade Group"을 "TASK 1"에 ResourceAssignment 객체를 생성하여 할당합니다.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// 조회가 포함된 사용자 정의 속성 정의를 생성합니다.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// 이 값은 MS Project의 "Resource usage" 보기에서 확인할 수 있습니다.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### 또 보기

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


