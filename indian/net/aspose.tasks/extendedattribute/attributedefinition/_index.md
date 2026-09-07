---
title: "ExtendedAttribute.AttributeDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute प्रॉपर्टी। एट्रिब्यूट परिभाषा प्राप्त करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/extendedattribute/attributedefinition/
---
## ExtendedAttribute.AttributeDefinition property

गुण परिभाषा प्राप्त करता है।

```csharp
public ExtendedAttributeDefinition AttributeDefinition { get; }
```

## उदाहरण

दिखाता है कि विस्तारित एट्रिब्यूट की एट्रिब्यूट परिभाषा को कैसे बदलें।

```csharp
var project = new Project();

// नया टास्क विस्तारित गुण परिभाषा बनाएं
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// एट्रिब्यूट में एक फ़ॉर्मूला जोड़ें।
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// विस्तारित एट्रिब्यूट बनाएं
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// एक नया तिथि विस्तारित एट्रिब्यूट परिभाषा बनाएं
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// एट्रिब्यूट में एक फ़ॉर्मूला जोड़ें।
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### संबंधित देखें

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


