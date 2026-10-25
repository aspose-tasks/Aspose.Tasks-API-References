---
title: "Task.ExtendedAttributes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task प्रॉपर्टी। विस्तारित एट्रिब्यूट के मानों को शामिल करने वाला ExtendedAttributeCollection ऑब्जेक्ट प्राप्त करता है"
type: docs
weight: 400
url: /hi/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

प्राप्त करता है ExtendedAttributeCollection ऑब्जेक्ट जिसमें विस्तारित गुण का मान शामिल है।

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## टिप्पणियाँ

दो डेटा टुकड़े आवश्यक हैं - विस्तारित एट्रिब्यूट तालिका की ओर एक pointer जो या तो unique ID या Field ID द्वारा निर्दिष्ट किया जाता है, और वह value जो या तो value के साथ निर्दिष्ट किया जाता है, या value list की ओर एक pointer।

## उदाहरण

दिखाता है कि टास्क विस्तारित एट्रिब्यूट कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// विस्तारित विशेषता परिभाषा बनाएं
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// शून्य इंडेक्स टास्क प्राप्त करें
var tsk = project.RootTask.Children.GetById(1);

// विस्तारित विशेषता जोड़ें
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// निम्नलिखित संक्षिप्त सिंटैक्स भी उपयोग किया जा सकता है: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Text1 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// इसे प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Attribute Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// जनरेट किए गए Extended Attribute को एक मान असाइन करें। एट्रिब्यूट का प्रकार "Text" है, "TextValue" प्रॉपर्टी का उपयोग किया जाना चाहिए।
taskExtendedAttributeText1.TextValue = "London";

// Extended Attribute को टास्क में जोड़ें
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Text2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// इसे प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Id 1 के लिए Text2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Extended Attribute को टास्क में जोड़ें
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Duration2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// परिभाषा को प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Id 3 के लिए Duration2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Extended Attribute को टास्क में जोड़ें
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Finish2 प्रकार की एक Extended Attribute Definition बनाएं
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// परिभाषा को प्रोजेक्ट के Extended Attributes संग्रह में जोड़ें
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Id 3 के लिए Finish2 Lookup Definition से एक Extended Attribute बनाएं
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Extended Attribute को टास्क में जोड़ें
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// टास्क के लिए विस्तारित एट्रिब्यूट्स पढ़ें
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### संबंधित देखें

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


