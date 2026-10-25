---
title: "ExtendedAttribute.ValueGuid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ExtendedAttribute. Mendapatkan guid dari nilai lookup"
type: docs
weight: 90
url: /id/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

Mendapatkan guid dari nilai lookup.

```csharp
public string ValueGuid { get; }
```

## Catatan

Tidak boleh diatur secara langsung, gunakan **ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue)** untuk membuat atribut yang diperluas dengan nilai lookup.

## Contoh

Menampilkan cara bekerja dengan GUID atribut yang diperluas.

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

// atribut yang diperluas memiliki GUID yang 
// sama dengan GUID dari bind 'Value' dari lookup
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### Lihat Juga

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


