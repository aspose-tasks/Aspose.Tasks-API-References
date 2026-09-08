---
title: "ExtendedAttribute.ValueGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttribute. Возвращает GUID значения справочника."
type: docs
weight: 90
url: /ru/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Получает GUID значения справочника.

```csharp
public string ValueGuid { get; }
```

## Примечания

Не следует устанавливать напрямую, вместо этого используйте ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) для создания расширенного атрибута со значением справочника.

## Примеры

Показывает, как работать с GUID расширенного атрибута.

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

// у расширенного атрибута есть GUID, который 
// равен GUID привязки 'Value' из справочника
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### См. также

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


