---
title: "ExtendedAttribute.ValueGuid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute प्रॉपर्टी। एक लुकअप मान का GUID प्राप्त करता है।"
type: docs
weight: 90
url: /hi/net/aspose.tasks/extendedattribute/valueguid/
---
## ExtendedAttribute.ValueGuid property

लुकअप मान का GUID प्राप्त करता है।

```csharp
public string ValueGuid { get; }
```

## टिप्पणियाँ

इसे सीधे सेट नहीं किया जाना चाहिए, इसके बजाय ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) का उपयोग करके लुकअप मान के साथ एक विस्तारित विशेषता बनाएं।

## उदाहरण

एक विस्तारित विशेषता GUID के साथ काम करने का तरीका दिखाता है।

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

// विस्तारित विशेषता का GUID है 
// जो लुकअप से बाइंड 'Value' के GUID के बराबर है
Console.WriteLine("Extended attribute GUID: " + attribute.ValueGuid);
Console.WriteLine("GUID of the first value in the lookup: " + value1.ValueGuid.ToString().ToUpper());
var guidFromString = Guid.Parse(attribute.ValueGuid);
Console.WriteLine("Are these GUIDs equal: " + guidFromString.Equals(value1.ValueGuid));
```

### संबंधित देखें

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


