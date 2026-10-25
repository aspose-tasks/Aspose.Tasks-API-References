---
title: "ExtendedAttribute.ValueGuid"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttribute özelliği. Bir arama değerinin GUID'ini alır."
type: docs
weight: 90
url: /tr/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Bir arama değerinin guid'ini alır.

```csharp
public string ValueGuid { get; }
```

## Açıklamalar

Doğrudan ayarlanmamalıdır, bunun yerine bir arama değeriyle genişletilmiş bir öznitelik oluşturmak için ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) kullanın.

## Örnekler

Bir genişletilmiş öznitelik GUID'iyle nasıl çalışılacağını gösterir.

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

// genişletilmiş öznitelik bir GUID'e sahiptir ve bu 
// arama'dan bağlanan 'Value' GUID'ine eşittir.
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


