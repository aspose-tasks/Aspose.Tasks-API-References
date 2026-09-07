---
title: "क्लास Value"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Value क्लास। मान सूची में एक मान का प्रतिनिधित्व करती है।"
type: docs
weight: 2800
url: /hi/net/aspose.tasks/value/
---
## Value class

मूल्य सूची में एक मान का प्रतिनिधित्व करता है।

```csharp
public class Value
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Value](value/)() | `Value` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | यदि इसे DateTime के रूप में दर्शाया जा सकता है तो वास्तविक मान प्राप्त करता या सेट करता है। डिफ़ॉल्ट मान MinValue है। |
| [Description](../../aspose.tasks/value/description/) { get; set; } | एक मान का विवरण प्राप्त करता या सेट करता है। |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Duration को दर्शाने के लिए उपयोग किए जाने वाले वास्तविक मान को प्राप्त करता या सेट करता है। |
| [Id](../../aspose.tasks/value/id/) { get; set; } | परियोजना में किसी मान का विशिष्ट पहचानकर्ता प्राप्त करता या सेट करता है। |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | संख्या या लागत मान को दर्शाने के लिए उपयोग किए जाने वाले वास्तविक मान को प्राप्त करता या सेट करता है। |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | कस्टम फ़ील्ड नाम के बारे में ध्वन्यात्मक जानकारी प्राप्त करता या सेट करता है। |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | टेक्स्ट स्ट्रिंग को दर्शाने के लिए उपयोग किए जाने वाले वास्तविक मान को प्राप्त करता या सेट करता है। |
| [Val](../../aspose.tasks/value/val/) { get; set; } | आंतरिक प्रतिनिधित्व में वास्तविक मान को प्राप्त करता या सेट करता है। नीचे सूचीबद्ध मजबूत टाइप्ड प्रॉपर्टीज़ का उपयोग करना पसंद करें। |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | एक GUID प्राप्त करता है जो पूरे प्रोजेक्ट में इस मान को अन्य मानों से पहचानता है। |

## उदाहरण

दिखाता है कि लुकअप मानों के साथ कैसे पढ़ें और काम करें।

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// टेक्स्ट प्रकार की विस्तारित एट्रिब्यूट परिभाषा बनाएं
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// अवधि प्रकार की विस्तारित एट्रिब्यूट परिभाषा बनाएं
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// विस्तारित एट्रिब्यूट परिभाषा के लिए लुकअप मान जोड़ें
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// तारीख प्रकार की विस्तारित एट्रिब्यूट परिभाषा बनाएं
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// संख्या प्रकार की विस्तारित एट्रिब्यूट परिभाषा बनाएं
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


