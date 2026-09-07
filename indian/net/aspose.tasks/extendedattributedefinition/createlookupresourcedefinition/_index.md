---
title: "ExtendedAttributeDefinition.CreateLookupResourceDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। एक फैक्टरी मेथड जो लुकअप के साथ एक विस्तारित एट्रिब्यूट डिफिनिशन बनाता है। इसमें CalculationType को Lookup सेट किया गया है और यह केवल Resources में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको fieldId और alias निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित एट्रिब्यूट डिफिनिशन बनाता है। इसमें [`CalculationType`](../calculationtype/) को Lookup सेट किया गया है और यह केवल Resources में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको *fieldId* और *alias* निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार field id से अनुमानित किया जाता है।

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | निर्दिष्ट [`ExtendedAttributeResource`](../../extendedattributeresource/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके लुकअप के साथ एक रिसोर्स के लिए कस्टम फ़ील्ड डिफिनिशन बनाएं और फिर इसे टेक्स्ट मानों से भरें:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

अद्यतन विस्तारित एट्रिब्यूट परिभाषाओं को कैसे लिखा जाए दिखाता है।

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// एक लुकअप और एक लुकअप मान के साथ नया text3 विस्तारित एट्रिब्यूट जोड़ें
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// एक लुकअप और दो लागत मानों के साथ नया cost1 विस्तारित एट्रिब्यूट जोड़ें
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// नया टास्क जोड़ें और एट्रिब्यूट लुकअप मान असाइन करें।
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// लुकअप के बिना एक अवधि एट्रिब्यूट परिभाषित करें।
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// नया टास्क जोड़ें और पहले परिभाषित अवधि एट्रिब्यूट को अवधि मान असाइन करें।
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### संबंधित देखें

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

फ़ैक्टरी मेथड जो लुकअप के साथ एक विस्तारित एट्रिब्यूट डिफिनिशन बनाता है। इसमें [`CalculationType`](../calculationtype/) को Lookup सेट किया गया है और यह केवल Resources में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको *customFieldType*, *fieldId* और *alias* निर्दिष्ट करना आवश्यक है।

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| customFieldType | CustomFieldType | निर्दिष्ट [`CustomFieldType`](../../customfieldtype/) प्रकार। |
| fieldId | ExtendedAttributeResource | निर्दिष्ट [`ExtendedAttributeResource`](../../extendedattributeresource/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *customFieldType*, *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके लुकअप के साथ एक रिसोर्स के लिए कस्टम फ़ील्ड डिफिनिशन बनाएं और फिर इसे टेक्स्ट मानों से भरें:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
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

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


