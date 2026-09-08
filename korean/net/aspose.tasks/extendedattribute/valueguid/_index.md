---
title: "ExtendedAttribute.ValueGuid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ExtendedAttribute 속성. 조회 값의 GUID를 가져옵니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

조회 값의 GUID를 가져옵니다.

```csharp
public string ValueGuid { get; }
```

## 비고

직접 설정해서는 안 되며, 대신 ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue)를 사용하여 조회 값을 가진 확장 속성을 생성하십시오.

## 예제

확장 속성 GUID를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "My lookup cost");
var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));

var value1 = new Value { NumericValue = 10000, Description = "Val 1", Id = 1 };
var value2 = new Value { NumericValue = 25000, Description = "Val 2", Id = 2 };

definition.AddLookupValue(value1);
definition.AddLookupValue(value2);

var attribute = definition.CreateExtendedAttribute(value1);

// 확장 속성에는 GUID가 있습니다 
// 'Value' 바인드의 조회에서 가져온 GUID와 같습니다.
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### 또 보기

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


