---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ExtendedAttributeDefinition मेथड। एक फैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट डिफिनिशन बनाता है जिसे Microsoft Project 'None' के रूप में दिखाता है। इसमें CalculationType को None सेट किया गया है और यह केवल Tasks में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको customFieldType, fieldId और alias निर्दिष्ट करना आवश्यक है।"
type: docs
weight: 40
url: /hi/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

फ़ैक्टरी मेथड जो एक सरल विस्तारित एट्रिब्यूट डिफिनिशन बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें [`CalculationType`](../calculationtype/) को None सेट किया गया है और यह केवल Tasks में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय आपको *customFieldType*, *fieldId* और *alias* निर्दिष्ट करना आवश्यक है।

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| customFieldType | CustomFieldType | निर्दिष्ट [`CustomFieldType`](../../customfieldtype/) प्रकार। |
| fieldId | ExtendedAttributeTask | निर्दिष्ट [`ExtendedAttributeTask`](../../extendedattributetask/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *customFieldType*, *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

दिखाता है कि टास्क के विस्तारित एट्रिब्यूट कैसे बनाएं।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Text1 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// इसे प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// प्रोजेक्ट में एक टास्क जोड़ें
var task = project.RootTask.Children.Add("Task 1");

// Attribute Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// जनरेट किए गए Extended Attribute को एक मान असाइन करें। एट्रिब्यूट का प्रकार "Text" है, "TextValue" प्रॉपर्टी का उपयोग किया जाना चाहिए।
taskExtendedAttributeText1.TextValue = "London";

// Extended Attribute को टास्क में जोड़ें
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Text2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// इसे प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// प्रोजेक्ट में एक टास्क जोड़ें
var task2 = project4.RootTask.Children.Add("Task 2");

// Id 1 के लिए Text2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Extended Attribute को टास्क में जोड़ें
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Duration2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// परिभाषा को प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// प्रोजेक्ट में एक टास्क जोड़ें
var task3 = project2.RootTask.Children.Add("Task 3");

// Id 3 के लिए Duration2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Extended Attribute को टास्क में जोड़ें
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Finish2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// परिभाषा को प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// प्रोजेक्ट में एक टास्क जोड़ें
var task4 = project3.RootTask.Children.Add("Task 4");

// Id 3 के लिए Finish2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Extended Attribute को टास्क में जोड़ें
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

फ़ैक्टरी मेथड जो एक सरल extended attribute definition बनाता है, जिसे Microsoft Project "None" के रूप में दिखाता है। इसमें [`CalculationType`](../calculationtype/) None के बराबर है और यह केवल टास्क में उपयोग किया जा सकता है। इस मेथड को कॉल करते समय *fieldId* और *alias* निर्दिष्ट करना आवश्यक है। फ़ील्ड प्रकार फ़ील्ड ID से अनुमानित होता है।

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | निर्दिष्ट [`ExtendedAttributeTask`](../../extendedattributetask/) फ़ील्ड ID। |
| उपनाम | स्ट्रिंग | निर्दिष्ट स्ट्रिंग उपनाम। |

### रिटर्न वैल्यू

निर्दिष्ट *fieldId* और *alias* के साथ [`ExtendedAttributeDefinition`](../) क्लास का इंस्टेंस बनाया गया।

## उदाहरण

इस उदाहरण का उपयोग करके एक कस्टम टेक्स्ट फ़ील्ड परिभाषा बनाएं:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

विस्तारित एट्रिब्यूट परिभाषा बनाने और एट्रिब्यूट के स्ट्रिंग मान को सेट करने का तरीका दिखाता है जबकि यह निर्मित हो रहा है।

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// विस्तारित एट्रिब्यूट को 'Common Info' के बराबर मान के साथ बनाएं
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// विस्तारित एट्रिब्यूट को 'Common Info' मान से इनिशियलाइज़ करके जोड़ें
task.ExtendedAttributes.Add(extendedAttribute);
```

### संबंधित देखें

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


