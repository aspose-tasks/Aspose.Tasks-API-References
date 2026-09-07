---
title: "ExtendedAttribute.FlagValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttribute प्रॉपर्टी। फ़्लैग प्रकार वाले एट्रिब्यूट के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान प्राप्त या सेट करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

'Flag' प्रकार वाले गुण के लिए फ़्लैग सेट है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool FlagValue { get; set; }
```

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | यदि [`AttributeDefinition`](../attributedefinition/) प्रॉपर्टी इनिशियलाइज़ नहीं है या वर्तमान एट्रिब्यूट फ़्लैग एट्रिब्यूट नहीं है तो थ्रो किया जाता है। |

## उदाहरण

बूलियन विस्तारित एट्रिब्यूट बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

// नया टास्क विस्तारित गुण परिभाषा बनाएं
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// एट्रिब्यूट में एक फ़ॉर्मूला जोड़ें।
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// विस्तारित एट्रिब्यूट बनाएं
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### संबंधित देखें

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


