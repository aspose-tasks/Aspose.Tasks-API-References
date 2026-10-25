---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। आंतरिक लुकअप सूची में एक मान जोड़ता है। यह ValueList के साथ हेरफेर करने का पसंदीदा तरीका है"
type: docs
weight: 300
url: /hi/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

आंतरिक लुकअप सूची में एक मान जोड़ता है। यह [`ValueList`](../valuelist/) के साथ हेरफेर करने का पसंदीदा तरीका है।

```csharp
public void AddLookupValue(Value value)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | मान | लुकअप में जोड़ने के लिए मान। |

## टिप्पणियाँ

यह मेथड केवल उन [`ExtendedAttributeDefinition`](../) इंस्टेंस के लिए काम करता है जिनका [`CalculationType`](../calculationtype/) Lookup के बराबर है।

## उदाहरण

नए Value को लुकअप सूची में जोड़ने के लिए इस कोड का उपयोग करें:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

दिखाता है कि असाइनमेंट्स के लिए लुकअप के साथ विस्तारित एट्रिब्यूट कैसे जोड़ें।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// एक ResourceAssignment ऑब्जेक्ट बनाकर संसाधन "1 TRG: Trade Group" को "TASK 1" को असाइन करें।
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// लुकअप के साथ कस्टम एट्रिब्यूट परिभाषा बनाएं।
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// यह मान MS Project के "Resource usage" दृश्य में देखा जा सकता है।
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// लुकअप के साथ कस्टम एट्रिब्यूट परिभाषा बनाएं।
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// यह मान MS Project के "Task usage" दृश्य में देखा जा सकता है।
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// गलत मानों को बाद में हटाया जा सकता है।
taskCostAttr.RemoveLookupValue(taskWrongValue);

// प्रोजेक्ट के साथ काम कर रहे हैं...
```

### संबंधित देखें

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


