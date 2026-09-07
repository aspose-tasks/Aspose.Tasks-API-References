---
title: "क्लास ParseErrorArgs"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ParseErrorArgs क्लास। ParseErrorCallback डेलीगेट के लिए डेटा प्रदान करता है"
type: docs
weight: 1240
url: /hi/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

[`ParseErrorCallback`](../parseerrorcallback/) डेलीगेट के लिए डेटा प्रदान करता है।

```csharp
public class ParseErrorArgs
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | स्ट्रिंग मान को पार्स करते समय उत्पन्न हुई अपवाद को प्राप्त करता है। |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | ऑब्जेक्ट फ़ील्ड का नाम प्राप्त करता है। |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | ऑब्जेक्ट फ़ील्ड का प्रकार प्राप्त करता है। |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | वह स्ट्रिंग मान प्राप्त करता है जिससे अपवाद उत्पन्न हुआ। |

## उदाहरण

अमान्य अक्षरों वाले XML फ़ाइल के साथ स्ट्रीम से प्रोजेक्ट पढ़ने का तरीका दिखाता है।

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // टूटा हुआ टाइमस्पैन वाला XML शामिल करने वाली फ़ाइल खोलें
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


