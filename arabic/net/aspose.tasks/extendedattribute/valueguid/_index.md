---
title: "ExtendedAttribute.ValueGuid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. تحصل على GUID لقيمة بحث."
type: docs
weight: 90
url: /ar/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

يحصل على الـ guid لقيمة البحث.

```csharp
public string ValueGuid { get; }
```

## ملاحظات

يجب عدم تعيينه مباشرةً، بل استخدم ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) لإنشاء سمة موسعة باستخدام قيمة بحث.

## الأمثلة

يوضح كيفية التعامل مع GUID لسمة موسعة.

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

// السمة الموسعة لديها GUID وهو 
// يساوي GUID للربط 'Value' من البحث
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### انظر أيضًا

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


